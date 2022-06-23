<template>
  <h1> Events for good </h1>
  <div class="events-container">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue';
// import axios from 'axios';

export default {
  name: 'EventList',
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 123,
          title: 'Cat Adoption Day',
          date: 'January 28, 2022',
          time: '12:00',
        },
        {
          id: 123,
          title: 'Cat Adoption Day',
          date: 'January 28, 2022',
          time: '12:00',
        },
        {
          id: 123,
          title: 'Cat Adoption Day',
          date: 'January 28, 2022',
          time: '12:00',
        },
      ],

    };
  },

};
</script>

<style scoped>
.events-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

</style>
