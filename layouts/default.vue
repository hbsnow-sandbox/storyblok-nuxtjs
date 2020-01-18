<template>
  <div :class="$style.app">
    <app-header />
    <main :class="$style.main">
      <nuxt />
    </main>
    <app-footer />
  </div>
</template>

<script>
import AppHeader from '~/components/app/AppHeader.vue'
import AppFooter from '~/components/app/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style>
@import '../assets/css/style.css';
</style>

<style module>
.app {
  display: flex;
  height: 100%;
  flex-direction: column;
}

.main {
  flex: 1 1 auto;
}
</style>
