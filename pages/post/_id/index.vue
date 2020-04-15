<template>
  <div id="postContent">
    <Header />
    <v-content>
      <v-container>
        <v-card class="py-4 px-4">
          <h1>Tiêu đề bài viết</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, expedita! Quis reiciendis maxime impedit excepturi tempore earum veniam natus quos possimus enim hic provident, illum at qui pariatur nemo velit.</p>
        </v-card>
      </v-container>
    </v-content>
  </div>
</template>
<script>
import Header from "~/components/header.vue";
export default {
  components: {
    Header
  }
};
</script>