<template>
    <div class="card mb-5">
      <div class="card-header has-background-primary">
        <h3 class="card-header-title is-centered has-text-white"> {{ event.title }} </h3>
      </div>
      <div class="card-content">
        <div class="content">
          @ {{ event.time }} on {{ event.date }}
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: "EventCard",
  props: {
    event: Object,
  }
};
</script>

<style scoped></style>
