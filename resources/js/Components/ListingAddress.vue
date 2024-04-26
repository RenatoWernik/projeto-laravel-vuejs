<template>
  Componente reutulizavel:
  <span>
  index: {{listing.id}}
  street: {{listing.street}} street number: {{listing.street_nr}}, 
  city: {{listing.city}}, for ${{listing.price}}
  </span>

</template>

<script setup>
  defineProps({
    listing: Object
  })
</script>