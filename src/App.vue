<script>
import AppHeader from './components/AppHeader.vue'
import AppProducts from './components/AppProducts.vue'
import AppMerch from './components/AppMerch.vue'
import AppUpperFooter from './components/AppUpperFooter.vue'
import AppLowerFooter from './components/AppLowerFooter.vue'

export default {
  components: {
    AppHeader,
    AppProducts,
    AppMerch,
    AppUpperFooter,
    AppLowerFooter,
  }
}
</script>

<template>
  <AppHeader/>

  <main>
    <AppProducts/>
    <AppMerch/>
  </main>

  <footer>
    <AppUpperFooter/>
    <AppLowerFooter/>
  </footer>
</template>

<style lang="scss">
  @use '../src/styles/partials/variables' as *;
  @use '../src/styles/partials/mixins' as *;
  @use './styles/general.scss' as *;
</style>
