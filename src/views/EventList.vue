<template>
  <div class="column is-half">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: 'EventList',
  components: {
    EventCard
  },
  data() {
    return {
      events: [{
        id: 1,
        title: 'My new event!',
        time: '12:00',
        place: 'Flaw City',
        date: '29/04/2021'
      },{        id: 2,
        title: 'Second event!',
        time: '13:00',
        place: 'Flaw City',
        date: '30/04/2021'}]
    }
  }
}
</script>
