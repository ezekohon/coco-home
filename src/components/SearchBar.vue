<template>
  <div class="bar">
    <span class="bar__text">¿Qué estás buscando?</span>
    <button class="bar__button">
      <search-icon />
    </button>
  </div>
</template>

<script>
import SearchIcon from '@/components/icons/SearchIcon.vue';

export default {
  name: "SearchBar",
  components: {
    SearchIcon,
  }
}
</script>

<style lang="stylus" scoped>
.bar
  width 100%
  height 45px
  display flex
  flex-direction row
  justify-content space-between
  align-items center
  background-color white
  border-radius 12px
  box-shadow 2px 2px 6px 0px rgba(202,202,202,0.69)

  &__text 
    font-size 14px
    font-weight 500
    line-height 20px
    margin-left 17px
    color #8CA2AE

  &__button
    background-color #FFC431
    margin 1px
    height 42px
    width 42px
    border-radius 12px
    border none

</style>