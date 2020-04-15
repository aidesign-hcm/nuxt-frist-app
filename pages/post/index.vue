<template>
  <div id="archive">
    <Header />
    <v-content>
      <v-container>
    <h1>trang post</h1>
    <v-row>
      <v-col md="4" cols="12">
          <postId />
      </v-col>
      <v-col md="4" cols="12">
          <postId />
      </v-col>
      <v-col md="4" cols="12">
          <postId />
      </v-col>
    </v-row>
  </v-container>
    </v-content></div>
</template>
<script>
import postId from './_id/index'
import Header from "~/components/header.vue";
export default {
    components:{
        postId,
        Header
    }
}
</script>