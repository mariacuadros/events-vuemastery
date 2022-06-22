<template>
  <h1> Events for good </h1>
  <div class="events-container">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue';

export default {
  name: 'HomeView',
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 59648,
          title: 'Cat adoption',
          time: '12:00pm',
          date: 'January 20, 2022',
        },
        {
          id: 59668,
          title: 'Cat adoption',
          time: '12:00pm',
          date: 'January 20, 2022',
        },
        {
          id: 58648,
          title: 'Cat adoption',
          time: '12:00pm',
          date: 'January 20, 2022',
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
