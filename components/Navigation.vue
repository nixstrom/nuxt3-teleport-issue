<template>
  <nav>
    <NuxtLink to="/">
      Page 1
    </NuxtLink>
    <NuxtLink to="/Page2">
      Page 2
    </NuxtLink>
  </nav>
</template>

<style>
a {
  text-decoration: none;
  margin: 0 1rem;
}
.router-link-active {
  border-bottom: solid 2px currentColor;
}
</style>
