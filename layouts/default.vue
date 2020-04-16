<template>
  <v-app>
    <nuxt />
    <v-footer fixed="fixed" app>
      <v-layout justify-center wrap>
        <span>&copy; {{ new Date().getFullYear() }}</span>
      </v-layout>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: "mr.3T"
    };
  },
  head(){
    return{
      titleTemplate: "%s Ai-Design Design and development",
      meta: [{
        hid: 'description',
        name: 'description',
        content: 'Home Page Ai Design have a content post',
      }]
    }
  },
  
};
</script>
