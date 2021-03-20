<template>
  <header class="header">
    <img class="header__logo" src="@/assets/images/banners/logo-coco.png" alt="Coco logo">
    <h1 class="header__title">Envía bienestar a tu <br/> familia en <span class="venezuela">Venezuela</span></h1>
    <img class="header__banner" src="@/assets/images/banners/prueba-banner-pagina.png" alt="Header banner">
    <search-bar class="header__search"/>
  </header>
</template>

<script>
import SearchBar from '@/components/SearchBar.vue';

export default {
  name: "AppHeader",
  components: {
    SearchBar,
  }
}
</script>

<style lang="stylus" scoped>
.header 
  position fixed
  display flex
  flex-direction column
  align-items flex-start
  left 0
  top 0
  width: 100%
  background linear-gradient(89.41deg, #0DBA72 2.6%, #0DBA72 99.38%);
  height 200px
  border-radius 0 0 30px 30px
  z-index 1

  &__logo
    margin-left 20px
    margin-top 26px
    margin-bottom 31px

  &__title 
    font-size 16px
    line-height 17.2px
    font-weight 400
    color white
    margin-left 20px
    text-align left
  
  &__banner 
    position absolute
    left 44%
    top 34%
    border-radius 0 0 30px 0
    z-index -1

  &__search
    max-width 85%
    align-self center
    position absolute
    top 90%

.venezuela
  font-weight 1000

</style>