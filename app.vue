<template>
  <div>
    <nuxt-layout>
      <NuxtPage />
    </nuxt-layout>
  </div>
</template>
<script>
import "@/assets/style.css";
</script>
<style scoped>
.page-enter-from {
  opacity: 0.6;
  transition: all, 1s;
  filter: blur(5rem);
}
/*/tablet/*/
@media (max-width: 991px) {
}
/*/mobile/*/
@media (max-width: 500px) {
}
</style>
