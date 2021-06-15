<template>
  <div class="fourth">
    <div class="fourth__fon-img"></div>
    <div class="fourth__shoe"></div>

    <div class="fourth__text-container">
      <div class="fourth__title">NIKE HYPERVENOM PHELON 3 FG</div>
      <div class="fourth__text">MEN'S FIRM-GROUND SOCCER CLEAT </div>
      <div class="fourth__buy-container">
        <div class="fourth__price"> $300</div>
        <q-btn class="button _blue fourth__btn" label="buy now"></q-btn>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component, } from 'vue-property-decorator'

@Component
export default class Fourt extends Vue {

}
</script>
<style lang='stylus'>
@import '../css/quasar.variables.styl'
.fourth
  width 100%
  position relative
  min-height 703px
  margin-top -270px
  align-items center
  justify-content center
  display flex
  padding 0 200px 
  &__fon-img
    background url('../assets/fon6.png')  no-repeat
    position absolute
    width 100%
    min-height 600px
    background-size cover
    z-index 10
    top -150px
  &__shoe
    top 100px
    background url('../assets/shoe-blue.png')  no-repeat
    margin-bottom: 220px
    width: 700px
    background-size: cover
    max-height: 300px
    min-height: 300px
    z-index: 11
  &__text-container
    position absolute
    bottom 0
    z-index 11
    left 200px
    padding-bottom 100px
  &__title
    font 700 35px/35px "Roboto",sans-serif
    margin-bottom 30px
  &__text
    font 300 20px/20px "Roboto",sans-serif
    color $txtDarkGray
  &__buy-container
    display flex
    align-items center
    margin-top 45px
  &__price
    font 700 35px/35px "Roboto",sans-serif
    color $txtRed 
    margin-right 30px
  &__btn
    min-width: 130px
    padding-top: 4px
    padding-bottom: 4px
</style>
