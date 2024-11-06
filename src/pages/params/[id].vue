<script setup lang="ts">
import { useRoute } from 'vue-router'

const route = useRoute('/params/[id]')

const params = route.params.id

console.log(params)
</script>

<template>
  <section>
    <!-- mandatory wrapper for transition vue-router -->
    <h1 class="text-6xl font-bold text-teal-500">Params Page</h1>
    <p class="mt-6">
      Params:
      <span class="ml-2 text-xl font-bold text-orange-600 dark:text-orange-400">
        {{ params }}
      </span>
    </p>
  </section>
</template>
