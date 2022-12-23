<template>
  <div class="card w-24 bg-primary shadow-xl">
  <figure ><img class="h-20" :src="'http://localhost:8000'+ item.icon" alt="Shoes" /></figure>
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