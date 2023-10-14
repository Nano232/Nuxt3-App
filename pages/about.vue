<template>
  <div>
    <header>
      <nav>
        <NuxtLink to="/">Nuxt</NuxtLink>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Doloremque
      officia fugiat voluptate aspernatur possimus suscipit laborum explicabo.
      Id, qui itaque?
    </p>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Doloremque
      officia fugiat voluptate aspernatur possimus suscipit laborum explicabo.
      Id, qui itaque?
    </p>
  </div>
</template>

<script setup>
name: "HomePage";
</script>

<style lang="scss" scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
