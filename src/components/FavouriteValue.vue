<template>
  <div class="favourite-value">
    <h2>Favourite Value</h2>
    <h4>The favourite value is: {{ favValue }}</h4>
    <h4>The normalized value: {{ normalizedVal }}</h4>
  </div>
</template>

<script>
export default {
  computed: {
    favValue() {
      return this.$store.state.counter;
    },
    normalizedVal() {
      return this.$store.state.normalizedCounter;
    },
  },
};
</script>

<style scoped>
.favourite-value {
  background-color: greenyellow;
  padding: 10px 20px;
  text-align: center;
  margin-bottom: 20px;
  color: rgb(255, 0, 0);
}
</style>
