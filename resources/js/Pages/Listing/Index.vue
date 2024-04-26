<template>
  pagina Index:

  <div v-for="(listing, index) in listings" v-bind:key="listing.id">
    <Link v-bind:href="`/listing/${listing.id}`">
      <ListingAddress v-bind:listing="listing" />  <!-- ListingAddress é um componente criado pois vai se repetir, esta na pasta "componentes" -->
     </Link>
  </div>

 
</template>

<script setup>
  import {Link} from "@inertiajs/vue3"
  import ListingAddress from "../../Components/ListingAddress.vue";

  defineProps({
    listings: Array,
  })

</script>