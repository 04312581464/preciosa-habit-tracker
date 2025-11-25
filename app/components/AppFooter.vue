<script setup lang="ts">
import { format } from 'date-fns';
const config = useRuntimeConfig();
const currentYear = format(new Date(), 'yyyy');
</script>

<template>
  <div class="mt-2 flex items-center justify-center gap-1 text-xs text-neutral-400">
    <a class="font-semibold transition hover:text-white" href="https://github.com/04312581464/preciosa-habit-tracker" target="_blank">Habit v{{ config.public.version }}</a>
    - by
    <a class="font-semibold transition hover:text-white" href="https://github.com/04312581464" target="_blank">Lalit Manjunatha</a>
    {{ currentYear }}
  </div>
</template>
