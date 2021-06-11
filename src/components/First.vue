<template>
  <div class="first">
    <div class="first__text-container">
      <div class="first__text">Your Title Goes Here Make It Long & Maybe 3 Lines</div>
      <div class="first__btn-container">
        <q-btn class="first__btn button" label="EXPLORE"></q-btn>
        <q-btn class="first__btn button" label="ADD TO CART"></q-btn>
      </div>
    </div>
    <div class="first__img-container">
      <div class="first__img-round _top"></div>
      <div class="first__img-round _bottom"></div>
      <div class="first__img-small-round _top"></div>
      <div class="first__img-small-round _bottom"></div>
      <div class="first__img-small-round _center"></div>
    </div>
    <div class="first__light"></div>
  </div>
</template>

<script lang="ts">
import { Vue, Component, } from 'vue-property-decorator'

@Component
export default class First extends Vue {

}
</script>
<style lang='stylus'>
@import '../css/quasar.variables.styl'
.first
  position relative
  padding  131px 117px
  width 100%
  min-height 903px
  background url('../assets/fon1.jpg')  no-repeat
  background-size cover
  display flex
  &__text-container
    padding 0 0 0 134px
    width 50%
  &__text
    max-width 430px
    color $txtBlue 
    font 400 40px/48px "Roboto",sans-serif
    padding 0 0 100px 0
  &__img-container
    margin-left -100px
    width 673px
    height 585px
    position: relative
    &:before
      content ''
      position absolute
      background url('../assets/shoe.png')  no-repeat
      background-size cover
      width 100%
      height 100%
      top 0
      z-index 12
      right 0
    &:after
      content ''
      position absolute
      background url('../assets/light.png')  no-repeat
      width 130%
      height 150%
      top -71px
      z-index 11
      right -85px
  &__img-round
    width 80px
    height 80px
    border-radius 50%
    background-color transparent
    border 3px solid $txtBlue 
    position absolute
    &._bottom
      bottom 0
      left -600px
    &._top
      top -50px
      right 0px
  &__img-small-round
    width 20px
    height 20px
    border-radius 50%
    background-color transparent
    border 3px solid $txtBlue 
    position absolute
    &._bottom
      bottom 0
      right  0px
    &._top
      top -50px
      left -600px
    &._center
      width 15px
      height 15px
      top 0px
      left 0
  &__btn-container
    display: flex
    max-width 400px
  &__btn
    width calc(50% - 15px)
    &:first-child
      margin-right 30px

</style>
