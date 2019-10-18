<template>
    <v-parallax :src="background">
        <v-container fluid>
          <v-card flat>
            <v-card-title>About 취운화</v-card-title>
            <v-card-text>
                lorem ipsum
                et cetra
            </v-card-text>
            <v-card-action>
            </v-card-action>
          </v-card>
        </v-container>
      </v-parallax>
</template>

<script>
import background from '../assets/vert_01.jpg';

export default {
  name: 'abouts',
  data() {
    return {
      background,
    };
  }
}
</script>