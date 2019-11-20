<template>
    <div class="container">
        <yandex-map
                    :coords="[54.62896654088406, 39.731893822753904]"
                    zoom="10"
                    style="width: 600px; height: 600px;"
                    :behaviors="['ruler']"
                    :controls="['trafficControl']"

                    map-type="map"
            >

        </yandex-map>
    </div>
</template>




<script>

export default {
}
</script>