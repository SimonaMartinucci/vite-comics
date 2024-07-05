<script>
import AppHeader from './components/AppHeader.vue'
import AppProducts from './components/AppProducts.vue'

export default {
  components: {
    AppHeader,
    AppProducts,
  }
}
</script>

<template>
  <AppHeader/>

  <main>
    <AppProducts/>
  </main>

</template>

<style lang="scss">
  @use '../src/styles/partials/variables' as *;
  @use '../src/styles/partials/mixins' as *;
  @use './styles/general.scss' as *;
</style>
