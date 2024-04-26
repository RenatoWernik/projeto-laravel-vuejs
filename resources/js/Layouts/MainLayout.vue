<template>
  Reactive Timer: {{counter}} <br>
  <Link href="/">Main Page</Link> <br>
  <Link href="/show">Show Page </Link> <br>
  <slot></slot>
</template>

<script setup>
  import { Link } from '@inertiajs/vue3'
  import {ref} from 'vue'
  const counter = ref(0)
  setInterval(() => counter.value++, 1000)
</script>

