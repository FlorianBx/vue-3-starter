<script setup lang="ts">
import { useRoute } from 'vue-router'

const route = useRoute()
const query = route.query.q

console.log(query)
</script>

<template>
  <section>
    <!-- mandatory wrapper for transition vue-router -->
    <h1 class="text-6xl font-bold text-teal-500">Search Page</h1>
    <p class="mt-6">
      Query params:
      <span class="ml-2 text-xl font-bold text-orange-600 dark:text-orange-400">
        {{ query }}
      </span>
    </p>
  </section>
</template>
