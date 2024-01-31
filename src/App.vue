<script>
import AppTitle from './components/AppTitle.vue'
import AppHero from './components/AppHero.vue'

export default {
  name: 'MyApp',
  components: {
    AppTitle,
    AppHero,
  }
}
</script>

<template>
  <div class="container">
    <AppTitle />
    <AppHero />
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 1000px;
  margin: 0 auto;
}
</style>