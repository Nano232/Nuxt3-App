<template>
  <div>
    <p>Products Details For {{ id }}</p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam ipsam
    dolorum quod aut nesciunt vero magni enim voluptatem pariatur quidem.
  </div>
</template>

<script setup>
const { id } = useRoute().params;
</script>

<style lang="scss" scoped></style>
