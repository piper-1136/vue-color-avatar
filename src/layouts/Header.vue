<template>
  <header class="header">
    <Logo />

    <h2 class="site-title">Color Avatar</h2>
  </header>
</template>

<script lang="ts" setup>
import Logo from '@/components/Logo.vue'
</script>

<style lang="scss" scoped>
@use 'src/styles/var';

.header {
  display: flex;
  align-items: center;
  height: var.$layout-header-height;
  padding: 1rem 2rem;

  .site-title {
    margin-left: 1rem;
    font-weight: bold;
    font-size: 1.9rem;
    cursor: default;

    @media screen and (max-width: var.$screen-sm) {
      display: none;
    }
  }
}
</style>
