<script>
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    AppHeader,
  }
}
</script>

<template>
  <AppHeader/>
</template>

<style lang="scss">
  @use '../src/styles/partials/variables' as *;
  @use '../src/styles/partials/mixins' as *;
  @use './styles/general.scss' as *;
</style>
