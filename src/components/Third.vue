<template>
  <div class="third">
    <div class="third__left-img"></div>
    <div class="third__right-img"></div>
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
    width 60%
    right: 0;
    top: -100px;
    position: absolute
    height 180%
</style>
