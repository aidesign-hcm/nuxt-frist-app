<template>
   <v-app-bar fixed app color="primary" dark>
      <v-toolbar-title>
        <v-btn to="/" text>{{title}}</v-btn>
      </v-toolbar-title>
      <v-spacer />
      <v-btn 
      v-for="link in links"
      :key="link.id"
      :to="link.url" 
      text 
      class="mr-2">{{link.label}}</v-btn>
      <v-btn
      @click="toggleTheme" text rounded>Light</v-btn>
    </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      title: "mr.3T",
      links:[
        {
          label:'Home',
          url:'/'
        },
        {
          label:'About',
          url:'/about'
        },
        {
          label:'Post',
          url:'/Post'
        },
        {
          label:'Dashboard',
          url:'/dashboard'
        },
        {
          label:'Admin',
          url:'/admin'
        },
        {
          label:'Login',
          url:'/login'
        },
        {
          label:'Register',
          url:'/signup'
        },
        
      ]
    };
  },
  methods: {
    toggleTheme() {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark;
    }
  }
}
</script>

<style>

</style>