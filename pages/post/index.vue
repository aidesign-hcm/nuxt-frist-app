<template>
  <div id="archive">
    <Header />
    <v-content>
      <v-container>
        <h1>trang post</h1>
        <EventCard
          v-for="(event, index) in events"
          :key="index"
          :event="event"
          :data-index="index"
        />
      </v-container>
    </v-content>
  </div>
</template>
<script>
import { mapState } from "vuex";
import EventCard from "@/components/EventCard.vue";
import Header from "~/components/header.vue";
export default {
  head() {
    return {
      title: "Post Archive",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Post Archive Ai Design have a content post"
        }
      ]
    };
  },
  async fetch({ store, error }) {
    try {
      await store.dispatch("events/fetchEvents");
    } catch (e) {
      error({
        statusCode: 503,
        message: "Unable to fetch events events at this time"
      });
    }
  },
  components: {
    Header,
    EventCard
  },
  computed: mapState({
    events: state => state.events.events
  })
};
</script>