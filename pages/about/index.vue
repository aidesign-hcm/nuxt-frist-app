<template>
  <div id="about-us">
    <Header />
    <v-content>
      <v-container>
        <v-card class="mx-auto" outlined>
          <v-list-item one-line>
            <v-list-item-content>
              <div class="overline mb-4">About</div>
              <v-list-item-title class="headline mb-1">Headline 5</v-list-item-title>
              <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-card>
      </v-container>
    </v-content>
  </div>
</template>

<script>
import Header from "~/components/header.vue";
export default {
  head(){
    return{
      title: "About Page",
      meta: [{
        hid: 'description',
        name: 'description',
        content: 'About Ai Design have a content post',
      }]
    }
  },
  components:{
    Header
  }
};

</script>

<style>
</style>