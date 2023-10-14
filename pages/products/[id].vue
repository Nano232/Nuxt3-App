<template>
  <div class="card">
    <div class="grid grid-cols-2 gap-10">
      <div class="p-7">
        <img :src="product.image" alt="image" class="mx-auto my-7" />
      </div>
      <div>
        <h2 class="text-4xl my-7">{{ product.title }}</h2>
        <p class="text-xl my-7">Price - ${{ product.price }}</p>
        <h3 class="font-bold border-b-2 mb-4 pb-2">Product Description</h3>
        <p class="mb-7">{{ product.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const url = "https://fakestoreapi.com/products/" + id;

const { data: product } = await useFetch(url, { key: id });

if (!product.value) {
  throw createError({ statusCode: 404, statusMessage: "Product Not Found" });
}

definePageMeta({
  layout: "products",
});
</script>

<style lang="scss" scoped>
img {
  max-width: 400px;
}
</style>
