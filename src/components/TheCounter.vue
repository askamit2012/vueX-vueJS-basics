<template>
  <div class="the-counter">
    <h3>The Count from getter is: {{ count }}</h3>
  </div>
</template>

<script>
export default {
  computed: {
    count() {
      return this.$store.getters.finalCounter;
    },
  },
};
</script>

<style scoped>
.the-counter {
  text-align: center;
  width: 60%;
  margin: 0 auto;
  padding: 5px 10px;
  background-color: rgb(255, 0, 200);
  color: #fff;
}
</style>
