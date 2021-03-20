<template>
  <div id="app">
    <app-header />

    <div class="home">
      <section class="home__selection mb-3">
        <market-selection />
      </section>
      <section class="home__cards" v-for="card in cards" :key="card.id">
        <card 
          :bannerImage="card.bannerImage"
          :bannerText="card.bannerText"
          :title="card.title"
          :subtitle="card.subtitle"
          :rating="card.rating"
          :shipping="card.shipping"
          :spend="card.spend"
          class="mb-5"
        >
        </card>
      </section>
    </div>

    <navigation-footer />
  </div>
</template>

<script>
import NavigationFooter from './components/NavigationFooter.vue'
import Card from './components/Card.vue'
import AppHeader from './components/AppHeader.vue'
import MarketSelection from './components/MarketSelection.vue'

export default {
  name: 'App',
  components: {
    NavigationFooter,
    Card,
    AppHeader,
    MarketSelection,
  },
  data () {
    return {
      cards: [
        {
          id: 1,
          bannerImage: 'Banner-20-Delicatck.png',
          title: 'Delicateck Caracas',
          subtitle: 'Supermercado',
          rating: 4.5,
          shipping: 3,
          spend: 'Gasta $ 80.000 para envio GRATIS'
        },
        {
          id: 2,
          bannerImage: 'Banner-20OFF-Lomas.png',
          title: 'Lomas Supermercados',
          subtitle: 'Supermercado',
          rating: 4.5,
          shipping: 3,
          spend: 'Gasta $ 80.000 para envio GRATIS'
        },
      ]
    }
  },
}
</script>

<style lang="stylus">
#app 
  font-family 'Poppins', sans-serif
  font-style normal
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50

.home
  position relative
  margin 230px 20px 110px 24px

.body 
  margin 0 0 86px 0
</style>

