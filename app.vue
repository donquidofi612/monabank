<template>
  <NuxtLayout>
    <NuxtLoadingIndicator />
    <!-- here -->
    <NuxtPage />
  </NuxtLayout>
</template>
<script setup lang="ts">

const getImagePath = (imageName: any) => {
  const publicPath = import.meta.env.BASE_URL || '/nuxt/';
  return `${publicPath}${imageName}`;
}
useHead({
  title: 'Mona Banq',
  // link: [{ rel: 'icon', type: 'image/png', href: getImagePath('images/brand-logos/favicon.ico') }]
})
</script>
<style>
.me-5 {
  margin-inline-end: 3rem !important;
}

:root {
  --primary-rgb: 190, 207, 66; /* Définit la couleur primaire en rouge */
}
</style>


<script lang="ts">
export default {
};
</script>