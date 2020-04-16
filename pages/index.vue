<template>
  <div id="home-page">
    <Header />
    <v-content>
      <v-container>
        <v-layout column justify-center align-center>
          <v-container>
            <v-row>
              <v-col md="4" cols="12">
                <nuxt-link :to="'/post/' + 1">
                  <v-card>
                    <v-img src="https://picsum.photos/510/300?random" aspect-ratio="1.7"></v-img>
                    <v-card-text>
                      <v-list-item-title class="headline mb-1">Headline 5</v-list-item-title>
                      <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
                    </v-card-text>
                  </v-card>
                </nuxt-link>
              </v-col>
              <v-col md="4" cols="12">
                <nuxt-link :to="'/post/' + 2">
                  <v-card>
                    <v-img src="https://picsum.photos/510/300?random" aspect-ratio="1.7"></v-img>
                    <v-card-text>
                      <v-list-item-title class="headline mb-1">Headline 5</v-list-item-title>
                      <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
                    </v-card-text>
                  </v-card>
                </nuxt-link>
              </v-col>
              <v-col md="4" cols="12">
                <nuxt-link :to="'/post/' + 3">
                  <v-card>
                    <v-img src="https://picsum.photos/510/300?random" aspect-ratio="1.7"></v-img>
                    <v-card-text>
                      <v-list-item-title class="headline mb-1">Headline 5</v-list-item-title>
                      <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
                    </v-card-text>
                  </v-card>
                </nuxt-link>
              </v-col>
            </v-row>
          </v-container>
        </v-layout>
      </v-container>
    </v-content>
  </div>
</template>

<script>
import Header from "~/components/header.vue";

export default {
  head(){
    return{
      title: "Home Page",
    }
  },
  
  components: {
    Header
  }
};
</script>
