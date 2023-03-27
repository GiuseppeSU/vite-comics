<script>
import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"
export default {
  components: {
    TheHeader,
    TheFooter,

  },
  data() {

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
      <div class="first-item">
        <img src="" alt="">

      </div>

    </div>

  </main>
  <TheFooter></TheFooter>
</template>

<style lang="scss">
@use "./styles/general.scss"
</style>
