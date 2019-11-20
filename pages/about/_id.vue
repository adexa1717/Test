<template>
    <div class="container">
        <h1> {{user.name}}</h1>
        <hr>
        <h4>{{user.email}}</h4>
    </div>
</template>


<script>
export default {
    validate({params}){
        return /^\d+$/.test(params.id)
    },

    async asyncData({$axios, params}){
        const user = await $axios.$get('https://jsonplaceholder.typicode.com/users/' + params.id)

        return {user}
    }
}
</script>