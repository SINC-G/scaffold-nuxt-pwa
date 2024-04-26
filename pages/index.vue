<script setup>
/* // If you want to use it in setup, import from the nuxtApp.
const {$pwa} = useNuxtApp();

const toast = useToast();

onMounted(() => {
  if ($pwa.offlineReady) toast.success("App ready to work offline");
}); */
</script>

<template>
  <div>
    <h1>Nuxt Vite PWA</h1>
    <ClientOnly> PWA Installed: {{ $pwa?.isPWAInstalled }} </ClientOnly>
    <NuxtLink to="/about"> About </NuxtLink>
  </div>
</template>

<style scoped></style>
