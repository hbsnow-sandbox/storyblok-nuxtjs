<template>
  <footer :class="$style.footer">
    <container>
      <footer :class="$style.container">
        Blog Example
      </footer>
    </container>
  </footer>
</template>

<script>
import Container from '~/components/shared/Container.vue'

export default {
  components: {
    Container
  }
}
</script>

<style module>
.footer {
  background: #eee;
}

.container {
  text-align: center;
  padding: 1rem 0;
}
</style>
