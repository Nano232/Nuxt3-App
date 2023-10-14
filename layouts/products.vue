<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4">
        <NuxtLink to="/products" class="font-bold">Nuxt Products</NuxtLink>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
      </nav>
    </header>

    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>
</template>
<style lang="scss" scoped>
.router-link-exact-active {
  color: #12b488;
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  ul {
    display: flex;
    gap: 30px;
    li {
      list-style-type: none;
      a {
        text-decoration: none;
      }
    }
  }
}
</style>
