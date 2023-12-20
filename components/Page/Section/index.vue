<script lang="ts" setup>
const { data } = await useFetch('/api-dsapi/query/all?community=openEuler')
</script>

<template>
  <section class="lg:px-8 px-4 mb-6">
    {{ data }}
    <slot />
  </section>
</template>
