<template>
  <div class="main-container">
    <OrderSummary />
  </div>
</template>

<script>
import OrderSummary from "./components/OrderSummary.vue";

export default {
  name: "App",
  components: {
    OrderSummary,
  },
};
</script>

<style lang="scss">
#app {
}

* {
  box-sizing: border-box;
  margin: 0;
}
</style>

<style lang="scss" scoped>
.main-container {
}
</style>
