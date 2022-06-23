<template>

<div class="event-card">
      <p class="event-card__date"> @ {{ event.time}} on {{ event.date }} </p>
      <p class="event-card__description"> {{ event.title }} </p>
</div>

</template>

<script>

export default {
  name: 'EventCard',

  props: {
    event: Object,
  },

};
</script>

<style scoped>

.event-card {
  border: 1px solid black;
  padding: 2em;
  width: 30%;
  cursor: pointer;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 1.5em;

;
}
.event-card:hover{
transform: scale(1.01);
box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}

.event-card__description{
  font-size: 1.5em;
  font-weight: bold;
}

</style>
