<script setup>

</script>

<template>
  <div class="bg-[rgb(10,10,50)] text-gray-100">
    <NuxtLoadingIndicator />
    <NuxtLayout>
      <Transition name="fade">
        <NuxtPage />
      </Transition>
    </NuxtLayout>
  </div>
</template>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-from {
  opacity: 0;
}
</style>
