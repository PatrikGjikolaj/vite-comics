<script>

import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}

</script>


<template>
  <div class="container-fluid p-0">
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>

