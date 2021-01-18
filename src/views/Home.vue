<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <counter />
    <counter-squared />
    <buttons />
    <color-code />
  </div>
</template>

<script>
import CounterSquared from "../components/CounterSquared.vue";
export default {
  name: "Home",
  components: {
    counter: require("@/components/Counter.vue").default,
    "counter-squared": require("@/components/CounterSquared.vue").default,
    buttons: require("@/components/Buttons.vue").default,
    "color-code": require("@/components/ColorCode.vue").default,
  },
};
</script>

<style>
div {
  margin-bottom: 20px;
}
.counter {
  font-size: 80px;
}
.buttons button {
  width: 50px;
  margin: 0 5px;
}
</style>
