<script setup lang="ts">
onMounted(() => {
  const token = getAuthToken()
  if (token) {
    navigateTo('/dashboard/links')
  }
  else {
    navigateTo('/dashboard/login')
  }
})
</script>

<template>
  <div />
</template>
