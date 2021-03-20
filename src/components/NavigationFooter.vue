<template>
  <nav class="nav">
    <a href="#" class="nav__link  nav__link--active">
      <market-icon/>
      <span class="nav__text">Tiendas</span>
    </a>
    <a href="#" class="nav__link">
      <location-icon/>
      <span class="nav__text">Caracas</span>
    </a>
    <a href="#" class="nav__link">
      <div class="nav__cart">
        <cart-icon/>
      </div>
    </a>
    <a href="#" class="nav__link">
      <dollar-icon/>
      <span class="nav__text">Gana $5.00</span>
    </a>
    <a href="#" class="nav__link">
      <user-icon/>
      <span class="nav__text">Iniciar sesión</span>
    </a>
  </nav>
</template>

<script>
// import DollarIcon from '@/assets/dollar-icon.svg';
import DollarIcon from '@/components/icons/DollarIcon.vue';
import MarketIcon from '@/components/icons/MarketIcon.vue';
import LocationIcon from '@/components/icons/LocationIcon.vue';
import CartIcon from '@/components/icons/CartIcon.vue';
import UserIcon from '@/components/icons/UserIcon.vue';
export default {
 name: 'NavigationFooter',
  components: {
    // DollarIcon,
    DollarIcon,
    MarketIcon,
    LocationIcon,
    CartIcon,
    UserIcon
  }
}
</script>

<style lang="stylus" scoped>
.nav
  position fixed
  display flex
  bottom 0
  right 0
  width 100%
  height 86px
  box-shadow 0 0 3px rgba(0, 0, 0, 0.2)
  background-color #ffffff
  overflow-x auto
  border-radius 20px 20px 0 0

  &__link
    display flex
    flex-direction column
    align-items center
    justify-content center
    flex-grow 1
    min-width 50px
    overflow hidden
    white-space nowrap
    font-size 13px
    color #444444
    text-decoration none
    -webkit-tap-highlight-color transparent
    transition background-color 0.1s ease-in-out

    &--active
      color #00AF71

  &__text
    font-size 10px
    color #8CA2AE

  &__cart
    box-shadow 2px 2px 6px 0px rgba(202,202,202,0.69)
    padding 15px
    border-radius 15px
    margin-bottom 35px
</style>

