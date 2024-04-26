<template>
  Pagina show:
  <div>
  <ListingAddress v-bind:listing="listing" />
  </div>
</template>

<script setup>
  import ListingAddress from "../../Components/ListingAddress.vue";
  defineProps({
    listing: Object
  })
</script>