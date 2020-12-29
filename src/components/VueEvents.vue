<template>
  <div>
    <header>
      <h1>Vue Events</h1>
    </header>
    <section id="events">
      <h2>Events in Action</h2>
      <button v-on:click="add()">Add</button>
      <button v-on:click="remove()">Remove</button>
      <p>Result: {{ counter }}</p>
    </section>
  </div>
</template>

<script>
export default {
  name: "VueEvents",
  data: () => {
    return {
      counter: 0
    };
  },
  methods: {
    add() {
      this.counter++;
    },
    remove() {
      this.counter--;
    },
  },
}
</script>

<style scoped>

</style>
