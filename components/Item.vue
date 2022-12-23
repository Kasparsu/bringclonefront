<template>
  <div class="card bg-primary shadow-xl p-2">
  <figure class="w-20 h-20 mx-auto"><img class="h-full" :src="'http://localhost:8000'+ item.icon" alt="Shoes" /></figure>
  <div class="card-body overflow-hidden m-0 p-0">
    <h2 class="card-title text-base mx-auto">{{item.name}}</h2>
    <p class="text-sm mx-auto break-keep h-4"></p>
  </div>
</div>
</template>

<script>
export default {
    props: ['item']
}
</script>

<style>

</style>