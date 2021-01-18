<template>
  <div>
    <input type="text" placeholder="Enter Type Text" v-model="colorCode" />
  </div>
</template>

<script>
export default {
  computed: {
    colorCode: {
      get() {
        return this.$store.state.colorCode;
      },
      set(newValue) {
        this.$store.dispatch("setColor", newValue);
      },
    },
  },
};
</script>

<style></style>
