<!-- <template>
  <div>
    <p v-if="user">Logged in as {{ user.username }}</p>
  </div>
</template>
<script setup>
  const user = useCookie('user')
  definePageMeta({
    middleware: function (to, from) {
      const authenticated = useCookie('user')
      if (!authenticated.value) {
        return navigateTo('/login')
      }
    }
  })
</script> -->

<!-- <template>
  <div>
    <h2>Index Page</h2>
    <p v-if="user">Logged in as {{ user.username }}</p>
  </div>
</template>

<script setup>
const user = useCookie('user')

definePageMeta({
  middleware: ['auth']
})
</script> -->

<template>
  <div>
    <h2>Index Page</h2>
    <p v-if="user">Logged in as {{ user.username }}</p>
  </div>
</template>

<script setup>
  const user = useCookie('user')
</script>