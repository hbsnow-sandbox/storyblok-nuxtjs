<template>
  <header :class="$style.header">
    <container>
      <div :class="$style.container">
        <h1 :class="$style.title">
          <nuxt-link :class="$style.link" to="/">Blog Example</nuxt-link>
        </h1>
        <div :class="$style.spacer"></div>
        <nav :class="$style.menu">
          <nuxt-link :class="$style.link" to="/ja/blog">Blog</nuxt-link>
        </nav>
        <nav :class="$style.language">
          <nuxt-link :class="$style.link" to="/ja/blog">JA</nuxt-link>
          <nuxt-link :class="$style.link" to="/en/blog">EN</nuxt-link>
        </nav>
      </div>
    </container>
  </header>
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
.header {
  background-color: rgba(0, 0, 0, 0.8);
  color: #fff;
  padding: 1rem 0;
}

.title {
  font-size: 1.5rem;
  margin: 0;
}

.link {
  color: #fff;
  padding: 0 0.25rem;
}

.container {
  display: flex;
  align-items: center;
  width: 100%;
}

.spacer {
  flex: 1 1 auto;
}

.menu {
  padding-right: 1rem;
}
</style>
