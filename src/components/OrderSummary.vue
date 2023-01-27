<template>
  <div class="root-container">
    <div class="main-container">
      <img
        alt="illustration-hero"
        class="illustration-hero-img"
        src="@/assets/illustration-hero.svg"
      />
      <div class="info-container">
        <h1 class="title">Order Summary</h1>
        <p class="description">
          You can now listen to millions of songs, audiobooks, and podcasts on
          any any device anywhere you like!
        </p>
      </div>
      <div class="padding-sides-1_5rem">
        <div class="plan-selection-container">
          <div class="plan-container">
            <img
              alt="icon-music"
              class="icon-music-img"
              src="@/assets/icon-music.svg"
            />
            <div class="billing-info-container">
              <p class="plan-title">Annual Plan</p>
              <p class="plan-price">$59.99/year</p>
            </div>
          </div>
          <a class="change-plan-link">Change</a>
        </div>
      </div>
      <div class="action-container">
        <button class="checkout-button">Proceed to Payment</button>
        <a class="cancel-link">Cancel Order</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OrderSummary",
  props: {},
};
</script>

<style lang="scss">
.padding-sides-1_5rem {
  width: 100%;
  padding: 0 1.5rem;
}
</style>

<style lang="scss" scoped>
@import "@/styles/_variables.scss";

.root-container {
}

.main-container {
  background-color: $white;
  max-width: 20.4375rem;
  margin: 0 1.5rem;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.illustration-hero-img {
  width: 100%;
  border-radius: 20px 20px 0 0;
}

.info-container {
  margin: 2rem 2rem 1.5rem 2rem;
}

.title {
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 900;
  font-size: 1.375rem;
  line-height: 29px;
  text-align: center;
  color: $dark_blue;
  margin-bottom: 1rem;
}

.description {
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 500;
  font-size: 0.9375rem;
  line-height: 25px;
  text-align: center;
  color: $desaturated_blue;
}

.plan-selection-container {
  background-color: $very_pale_blue;
  margin-bottom: 1.5rem;
  padding: 1rem;
  border-radius: 11px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.plan-container {
  display: flex;
  flex-direction: row;
  align-items: center;
}

.icon-music-img {
  width: 3rem;
  height: 3rem;
  margin-right: 1.25rem;
}

.billing-info-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-right: 3.125rem;
}

.plan-title {
  margin-bottom: 0.1875rem;
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 900;
  font-size: 0.875rem;
  line-height: 19px;
  color: $dark_blue;
}

.plan-price {
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 500;
  font-size: 0.875rem;
  line-height: 19px;
  color: $desaturated_blue;
}

.change-plan-link {
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 700;
  font-size: 0.8125rem;
  line-height: 17px;
  text-decoration-line: underline;
  text-underline-position: under;
  color: $faded_purple;
}

.change-plan-link:hover {
}

.action-container {
  width: 100%;
  padding: 0 1.5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.checkout-button {
  width: 100%;
  margin-bottom: 1.5rem;
  padding: 1rem 4rem;
  background-color: $bright_blue;
  box-shadow: 0 20px 20px rgba(56, 42, 225, 0.190291);
  border-width: 0;
  border-radius: 11px;
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 900;
  font-size: 0.9375rem;
  line-height: 20px;
  color: $white;
}

.checkout-button:hover {
  background-color: $faded_purple;
}

.cancel-link {
  margin-bottom: 2rem;
  font-family: "Red Hat Display", serif;
  font-style: normal;
  font-weight: 900;
  font-size: 0.9375rem;
  line-height: 20px;
  color: $desaturated_blue;
}

.cancel-link:hover {
  color: $dark_blue;
}
</style>
