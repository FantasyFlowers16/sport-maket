<template>
  <div class="third">
    <div class="third__shoes-img"></div>
    <div class="third__left-img"></div>
    <div class="third__right-img"></div>
    <div class="third__text-container">
      <div class="third__title">The Way You Like It</div>
      <div class="third__text">Lorem ipsum dolor sit amet, 
        consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
        Ut enim ad minim veniam, quis nostrud exercitation </div>
        <q-btn class="button _blue" label="buy now"></q-btn>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component, } from 'vue-property-decorator'

@Component
export default class Third extends Vue {

}
</script>
<style lang='stylus'>
@import '../css/quasar.variables.styl'
.third
  width 100%
  position relative
  min-height 903px
  margin-top -270px
  display flex
  &__left-img
    background url('../assets/fon4.png')  no-repeat
    width 40%
    height 100%
    min-height 700px
  &__right-img
    background url('../assets/fon5.png')  no-repeat
    background-size: cover
    width 39%
    right 0
    top -250px
    z-index 3
    position: absolute
    height 106%
    left 25%
  &__shoes-img
    background url('../assets/shoe-double.png')  no-repeat
    width  620px
    height 243px
    z-index 10
    background-size cover
    position absolute
    top 200px
    left 240px
    margin-top 100px
  &__text-container
    margin-left 250px
    max-width 550px
    position relative
    display flex
    flex-direction column
    justify-content center
    align-items center
    margin-bottom 250px
    z-index: 11
  &__title
    width 100%
    font 700 60px/60px "Roboto",sans-serif
    text-align: center
    margin-bottom 50px
  &__text
    width 100%
    text-align: center
    font 300 20px/35px "Roboto",sans-serif
    margin-bottom 25px
</style>
