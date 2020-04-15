<template>
  <div id="login">
    <Header />
    <v-content>
      <v-container>
        <v-card width="600" class="mx-auto px-2 py-2">
          <v-card-title>
            <h1 class="display-1">Login</h1>
          </v-card-title>
          <v-card-text>
            <v-form>
              <v-text-field label="username" prepend-icon="mdi-account-circle" />
              <v-text-field
                :type="showPassword ? 'text' : 'password'"
                label="password"
                prepend-icon="mdi-lock"
                :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
                @click:append="showPassword =! showPassword"
              />
            </v-form>
          </v-card-text>
          <v-divider></v-divider>
          <v-card-actions>
            <v-btn color="success">Resgister</v-btn>
            <v-spacer />
            <v-btn color="info">Login</v-btn>
          </v-card-actions>
        </v-card>
      </v-container>
    </v-content>
  </div>
</template>
<script>
import Header from "~/components/header.vue";
export default {
  data() {
    return {
      showPassword: false
    };
  },
  components:{
      Header
  }
};
</script>

<style>
</style>