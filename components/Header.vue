<template>
  <header class="header">
    <NuxtLink to="/" class="header__link">Home</NuxtLink>
    <NuxtLink to="/contact" class="header__link">Contact</NuxtLink>
  </header>
</template>

<style scoped>
.header {
  position: sticky;
  position: fixed;
  display: flex;
  flex-direction: column;
  align-items: center;
  right: 0;
  width: 40pt;
}
.header__link {
  writing-mode: vertical-lr;
  margin: 10pt 0;
  font-size: 1.4em;
}
</style>
