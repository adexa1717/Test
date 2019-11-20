<template>
    <div class="container">
        <yandex-map
                    :coords="[43.2601815, 76.9325566]"
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