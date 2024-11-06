<script setup lang="ts">
import { useDark, useToggle } from '@vueuse/core'

const isDark = useDark()
const toggleDark = useToggle(isDark)
</script>

<template>
  <div class="min-h-screen bg-slate-100 dark:bg-slate-900 text-slate-900 dark:text-slate-100">
    <header class="px-6 py-3">
      <nav class="flex justify-end">
        <ul class="flex space-x-4">
          <li><router-link class="hover:text-teal-500" to="/">Home</router-link></li>
          <li><router-link class="hover:text-teal-500" to="/about">About</router-link></li>
          <li><router-link class="hover:text-teal-500" to="/params/1">Params</router-link></li>
          <li>
            <router-link class="hover:text-teal-500" to="/search?q=hello">Search</router-link>
          </li>
          <li>
            <button @click="toggleDark()">
              {{ isDark ? '💡' : '☀️' }}
            </button>
          </li>
        </ul>
      </nav>
    </header>

    <main class="p-6">
      <slot />
    </main>

    <footer class="p-6"></footer>
  </div>
</template>
