<template>
    <v-container>
        <v-flex>
            <v-img :src="feedUrl" :aspect-ratio="320/240"></v-img>
        </v-flex>
    </v-container>
</template>
<script>
export default {
  computed: {
    feedUrl() {
      return process.env.VUE_APP_WEBCAM_URL;
    }
  }
};
</script>
