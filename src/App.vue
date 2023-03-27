<script>
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"
export default {
  components: {
    TheHeader,
    TheFooter,

  },
  data() {
    return {

    }

  },
  methods: {

  }
}
</script>

<template>
  <TheHeader></TheHeader>

  <main>
    <div class="content">
      <h1>Il contenuto va qui!</h1>
    </div>

    <div class="container-mid">
      <div class="container-items">
        <div class="first-item">
          <img src="./assets/buy-comics-digital-comics.png" alt="Digital comics">
          <h3>Digital Comics</h3>
        </div>

        <div class="first-item">
          <img src="./assets/buy-comics-merchandise.png" alt="Merchandise">
          <h3>Dc Merchandise</h3>
        </div>

        <div class="first-item">
          <img src="./assets/buy-comics-subscriptions.png" alt="Subscription">
          <h3>Subscription</h3>
        </div>

        <div class="first-item">
          <img src="./assets/buy-comics-shop-locator.png" alt="shop-locator">
          <h3>Comic Shop Locator</h3>
        </div>

        <div class="first-item">
          <img src="./assets/buy-dc-power-visa.svg" alt="Power">
          <h3>Dc Power Visa</h3>
        </div>
      </div>
    </div>

  </main>
  <TheFooter></TheFooter>
</template>

<style lang="scss">
@use "./styles/general.scss"
</style>
