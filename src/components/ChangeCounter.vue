<template>
  <button @click="addFive">Add Five</button>
</template>

<script>
export default {
  methods: {
    addFive() {
      //   this.$store.state.counter += 10;
      //   this.$store.commit('increase', 5);
      this.$store.commit({
        type: 'increase',
        value: 5,
      });
    },
  },
};
</script>

<style></style>
