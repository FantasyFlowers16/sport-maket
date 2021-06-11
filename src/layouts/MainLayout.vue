<template>
  <q-layout view="lHh Lpr lFf">
    <q-header >

    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">

import { Vue, Component } from 'vue-property-decorator'

@Component({
  components: {  }
})
export default class MainLayout extends Vue {
}
</script>
