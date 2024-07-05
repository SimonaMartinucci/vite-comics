<script>
import AppHeader from './components/AppHeader.vue'
import AppProducts from './components/AppProducts.vue'
import AppMerch from './components/AppMerch.vue'

export default {
  components: {
    AppHeader,
    AppProducts,
    AppMerch,
  }
}
</script>

<template>
  <AppHeader/>

  <main>
    <AppProducts/>
    <AppMerch/>
  </main>

</template>

<style lang="scss">
  @use '../src/styles/partials/variables' as *;
  @use '../src/styles/partials/mixins' as *;
  @use './styles/general.scss' as *;
</style>
