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
@import "@/styles/_variables.scss";

* {
  box-sizing: border-box;
  margin: 0;
}

#app {
  background-image: url("@/assets/pattern-background-mobile.svg");
  background-repeat: no-repeat;
  background-color: $pale_blue;
  background-size: 100% auto;
  font-family: "Red Hat Display", serif;
  font-size: 1rem;
}

@media only screen and (min-width: 1440px) {
  #app {
    background-image: url("@/assets/pattern-background-desktop.svg");
  }
}
</style>

<style lang="scss" scoped>
.main-container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>
