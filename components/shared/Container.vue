<template>
  <div :class="$style.container"><slot /></div>
</template>

<style module>
.container {
  width: 100%;
  max-width: 950px;
  padding: 0 1rem;
  margin: 0 auto;
}
</style>
