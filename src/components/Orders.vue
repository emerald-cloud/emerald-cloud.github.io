<template>
    <v-parallax :src="background">
        <v-container fluid>
          <v-card flat>
            <v-card-title>Order:주문하기</v-card-title>
          </v-card>
        </v-container>
    </v-parallax>
</template>

<script>
import background from '../assets/vert_02.jpg'
export default {
    name: 'orders',
    data() {
        return {
            background,
        }
    }
}
</script>