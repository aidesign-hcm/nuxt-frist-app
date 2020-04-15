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
  
};
</script>
