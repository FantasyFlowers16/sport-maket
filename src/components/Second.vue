<template>
  <div class="second">
    <div class="second__fon1"></div>
    <div class="second__fon2"></div>
    <div class="second__img-conainer">
      <div class="second__img"></div>
      <div class="second__lines"></div>
      <div class="second__text _left">Your Awesome Text</div>
      <div class="second__text _right">Your Awesome Text</div>
      <div class="second__text _top">Your Awesome Text</div>
      <q-btn class="second__btn button" label="buy now"></q-btn>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component, } from 'vue-property-decorator'

@Component
export default class Second extends Vue {

}
</script>
<style lang='stylus'>
.second
  margin-top -215px
  width 100%
  min-height 1530px
  position relative
  display: flex
  justify-content: center;
  &__fon1
    background url('../assets/fon2.png')  no-repeat
    background-size cover
    position absolute
    height 100%
    width 100%
    top 0
    z-index 5
  &__fon2
    content ''
    position absolute
    width 100%
    left 0px
    background url('../assets/fon3.png')  no-repeat
    background-size cover
    height 106%
    top -46px
  &__img-conainer
    position relative
    margin-top 300px
    width 600px
    height 550px
    z-index 6
  &__img
    background url('../assets/shoe-white.png')  no-repeat
    background-size: cover
    width 100%
    height 100%
  &__lines
    background url('../assets/lines.png')  no-repeat
    background-size: cover
    width 130%
    height 68%
    z-index 1
    position absolute
    top: 67px
    left: -85px
    heigh 550px
    // transform: scale(0.45)
  &__text
    color $txtBlue
    font 400 20px/20px "Roboto",sans-serif
    position absolute
    width: 100%
    &._left
      top 130px 
      left -190px
    &._top
      top 20px
      left 460px
    &._right
      text-align: right
      bottom 330px 
      right -170px
  &__btn
    bottom 70px
    left: -200px
    position absolute
</style>
