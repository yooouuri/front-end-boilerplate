<script setup lang="ts">
const props = defineProps<{
  title: string
}>()
</script>

<template>
  <section class="rounded shadow bg-slate-200 dark:bg-slate-800 border border-slate-800 dark:border-slate-200">
    <header class="border-t border-b-slate-800 dark:border-b-slate-200 p-4 border-b">
      <h2 class="text-center text-2xl font-bold tracking-wide text-slate-700 dark:text-slate-300">
        {{ props.title }}
      </h2>
    </header>
    <main class="p-4">
      <slot />
    </main>
  </section>
</template>
