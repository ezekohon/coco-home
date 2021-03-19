<template>
  <div class="card">
    <img class="card__image" src="@/assets/images/banners/Banner-20-Delicatck.png" alt="Placeholder image">
    <div class="card__content">
      <p class="card__title mb-0">John Smith</p>
      <div class="card__market my-0">
        <p class="card__subtitle mr-3 my-0">Supermercado</p>
        <star-icon class="mr-1"/>
        <p class="card__subtitle my-0">4.5</p>
      </div>
      <div class="card__legend mt-0 mb-3">
        <delivery-icon class="mr-1"/>
        <p class="card__shipping my-0 mr-1">3 days</p>
        <span class="mr-1">&#183;</span>
        <p class="card__spend my-0">dsad</p>
      </div>
    </div>
  </div>
</template>

<script>
import StarIcon from '@/components/icons/StarIcon.vue';
import DeliveryIcon from '@/components/icons/DeliveryIcon.vue';

export default {
  name: "Card",
  components: {
    StarIcon,
    DeliveryIcon,
  },
  props: { 
    bannerImage: {
      type: String,
      required: true,
    },
    bannerText: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    subtitle: {
      type: String,
      required: true,
    },
    rating: {
      type: Number,
      required: true,
    },
    shipping: {
      type: Number,
      required: true,
    },
    spendLegend: {
      type: String,
      required: true,
    },
  }
}
</script>

<style lang="stylus" scoped>
.card
  display flex
  flex-direction column
  min-width 0
  border-radius 20px
  box-shadow 2px 2px 6px 0px rgba(202,202,202,0.69)

  &__image
    height 165px
    width 100%
    display block;
    border-radius 20px 20px 0 0 

  &__content
    display flex
    flex-direction column
    align-items flex-start
    padding-left 25px
  
  &__title 
    font-size 16px
    font-weight 600
    line-height 20px

  &__market 
    display flex
    flex-direction row
    align-items center
  
  &__subtitle 
    font-size 12px
    font-weight 400
    line-height 20px    

  &__legend
    display flex
    flex-direction row
    align-items center
  
  &__shipping
    font-size 11px
    font-weight 400
    line-height 20px

  &__spend
    font-size 11px
    font-weight 500
    line-height 20px
</style>