<template>
    <v-carousel show-arrows hide-delimiters cycle>
        <v-carousel-item v-for="(s,si) in slides" :key="`slide-image-${si}`">
            <img :src="s" width="100%" resize />
        </v-carousel-item>
    </v-carousel>
</template>

<script>

export default {
    name: 'slides',
    computed: {
        slides() {
            return this.slide_pathes.map((path) => require(`../assets/${path}`));
        }
    },
    data() {
        return {
            slide_pathes: [
                'rect_01.jpg',
                'rect_02.jpg',
                'rect_03.jpg',
                'rect_04.jpg',
                'rect_05.jpg',
                'rect_06.jpg',
                'rect_07.jpg',
                'rect_08.jpg',
                'rect_09.jpg',
                'rect_10.jpg',
            ],
        }
    }
}
</script>