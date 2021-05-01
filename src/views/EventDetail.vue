<template>
    <div v-if="event" class="block mt-5">
        <h3 class="title pb-4 is-size-1"> {{ event.title }} </h3>
        <h4 class="subtitle"> @ {{ event.time }} on {{ event.date }} </h4>
        <h5> {{ event.description }} </h5>
    </div>
</template>

<script>

import EventService from "@/services/EventService.js";

export default {
  name: "EventDetail",
  props: ['id'],
  data() {
      return {
          event: null,
      }
  },
  created(){
    EventService.getEvent(this.id)
    .then(response => this.event = response.data)
    .catch(error => console.log(error))
  }
};
</script>

<style scoped></style>
