<template>
  <q-page class="row items-center justify-evenly">
   <first></first>
   <second></second>
   <third></third>
   <fourth></fourth>
  </q-page>
</template>

<script lang="ts">
import First from 'components/First.vue'
import Second from 'components/Second.vue'
import Third from 'components/Third.vue'
import Fourth from 'components/Fourth.vue'
import { Vue, Component } from 'vue-property-decorator'

@Component({
  components: { First, Second, Third, Fourth }
})
export default class PageIndex extends Vue {
}
</script>
