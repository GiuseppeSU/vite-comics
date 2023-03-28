<script>
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"
import ProductList from "./components/ProductList.vue"

export default {
  components: {
    TheHeader,
    TheFooter,
    ProductList



  },
  data() {
    return {
      imageName: [
        {
          img: 'buy-comics-digital-comics.png',
          text: 'Digital Comics'

        },
        {
          img: 'buy-comics-merchandise.png',
          text: 'Dc Merchandise'

        },

        {
          img: 'buy-comics-subscriptions.png',
          text: 'Subscription'

        },
        {
          img: 'buy-comics-shop-locator.png',
          text: 'Comic Shop Locator'

        },
        {
          img: 'buy-dc-power-visa.svg',
          text: 'Dc Power Visa'

        },


      ],

    }

  },
  methods: {
    getImagePath: function (img) {
      console.log(img)
      return new URL(`./assets/${img}`, import.meta.url).href;

    }
  }
}
</script>

<template>
  <TheHeader></TheHeader>

  <main>
    <ProductList></ProductList>


    <div class="container-mid">
      <div class="container-items">
        <div class="first-item" v-for="(img, index) in imageName">
          <img :src="getImagePath(img.img)" alt="Digital comics">
          <h3>{{ img.text }}</h3>
        </div>
      </div>
    </div>



  </main>
  <TheFooter></TheFooter>
</template>

<style lang="scss">
@use "./styles/general.scss"
</style>
