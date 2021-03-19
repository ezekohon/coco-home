<template>
  <nav class="nav">
    <a href="#" class="nav__link">
      <market-icon/>
      <span class="nav__text">Tiendas</span>
    </a>
    <a href="#" class="nav__link nav__link--active">
      <location-icon/>
      <span class="nav__text">Caracas</span>
    </a>
    <a href="#" class="nav__link">
      <cart-icon/>
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
  position: fixed
  bottom: 0
  right: 0
  width: 100%
  height: 86px
  box-shadow: 0 0 3px rgba(0, 0, 0, 0.2)
  background-color: #ffffff
  display: flex
  overflow-x: auto
  border-radius: 20px 20px 0 0

.nav__link
  display: flex
  flex-direction: column
  align-items: center
  justify-content: center
  flex-grow: 1
  min-width: 50px
  overflow: hidden
  white-space: nowrap
  font-size: 13px
  color: #444444
  text-decoration: none
  -webkit-tap-highlight-color: transparent
  transition: background-color 0.1s ease-in-out

.nav__link:hover
  background-color: #eeeeee

.nav__link--active
  color: #009578

.nav__icon
  font-size: 18px

.nav__text
  font-size: 10px
  color: #8CA2AE
</style>

