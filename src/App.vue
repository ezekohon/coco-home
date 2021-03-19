<template>
  <div id="app">
    <navigation-footer />
    <div class="content">
      <div ></div>
      <card />
    </div>
  </div>
</template>

<script>
import NavigationFooter from './components/NavigationFooter.vue'
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    NavigationFooter,
    Card
  },
  data () {
    return {
      cards: [
        {
          bannerImage: 'Banner-20-Delicatck.png',
          bannerText: '',
          title: 'Delicateck Caracas',
          subtitle: 'Supermercado',
          rating: 4.5,
          shipping: '3 días',
          spend: 'Gasta $ 80.000 para envio GRATIS'
        },
        {
          bannerImage: 'Banner-20OFF-Lomas.png',
          bannerText: '',
          title: 'Lomas Supermercados',
          subtitle: 'Supermercado',
          rating: 4.5,
          shipping: '3 días',
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
  margin-top 60px

.content
  position relative
  margin 0 20px 0 24px

.body {
  margin 0 0 86px 0
}

</style>

