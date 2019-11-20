<template>
    <div class="container">
        <h1>{{pageTitle}}</h1>

        <ul>
            <li v-for="user of users" :key="user.id">
                <a href="#" @click.prevent="openAbout(user)">{{user.name}}</a>
            </li>
        </ul>        
    </div>
</template>

<script>
export default {
    async asyncData({$axios}){
        const users = await $axios.$get('https://jsonplaceholder.typicode.com/users')
        return {users}
    },
    data: () =>({
        pageTitle:'О нас'
    }),
    methods:{
        openAbout(user) {
            this.$router.push('/about/' + user.id)
        }
    }
}
</script>