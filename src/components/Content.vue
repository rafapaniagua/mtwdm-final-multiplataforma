<template>
  <section>
    <Banner />
  </section>
  <section>
    <About />
  </section>
  <section class="cards">
    <template v-for="cardItem, index in cardItems" :key="index">
      <Card :cardItem="cardItem" />
    </template>
  </section>
</template>

<script>
import Banner from './Banner.vue'
import About from './About.vue'
import Card from './Card.vue'

export default {
  data() {
    return {
      cardItems: JSON.parse(localStorage.getItem('cardItems'))
    }
  },
  components: {
    Banner,
    About,
    Card
  }
}
</script>

<style>

</style>