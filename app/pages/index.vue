<script setup lang="ts">
const { getToken } = useAuthToken()

onMounted(() => {
  const token = getToken()
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
