<template>
  <div class="selection">
    <h3 class="selection__title mb-2">Selecciona tu tienda</h3>
    <span class="selection__location mb-3"><location-icon-2 class="mr-1"/> <span>Caracas, Ajuro</span></span>
    <div class="selection__types">
      <div class="selection__supermarket">
        <supermarket-icon />
        <span>Supermercados</span>
      </div>
      <div class="selection__butchershop">
        <butcher-shop-icon />
        <span>Carnicerías</span>
      </div>
      <div class="selection__farmacy">
        <farmacy-icon />
        <span>Farmacias</span>
      </div>
    </div>
  </div>
</template>

<script>
import LocationIcon2 from '@/components/icons/LocationIcon2.vue';
import SupermarketIcon from '@/components/icons/SupermarketIcon.vue';
import ButcherShopIcon from '@/components/icons/ButcherShopIcon.vue';
import FarmacyIcon from '@/components/icons/FarmacyIcon.vue';
export default {
  components: {
    LocationIcon2,
    SupermarketIcon,
    ButcherShopIcon,
    FarmacyIcon,
  }
}
</script>

<style lang="stylus" scoped>
.selection
  display flex
  flex-direction column
  align-items flex-start

  &__title 
    font-size 20px
    font-weight 600
    line-height 28px
    color #44535B

  &__location
    display flex
    color #00AF71
    align-items center
    font-size 16px
    font-weight 600

  &__types
    display flex
    flex-direction row
    width 100%
    justify-content space-evenly
    font-size 12px
    font-weight 600
    line-height 20px

  &__supermarket 
    display flex
    flex-direction column
    align-items center
    color #00AF71

  &__butchershop 
    display flex
    flex-direction column
    align-items center
    font-weight 500

  &__farmacy
    display flex
    flex-direction column
    align-items center
    font-weight 500
</style>