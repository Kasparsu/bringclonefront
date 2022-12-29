<template>
  <div class="bg-primary shadow-xl">
    <div class="flex justify-center pt-2 h-[60px] items-center"><img class="max-h-[50px] max-w-[65px] h-fit" :src="'http://localhost:8000'+ item.icon" :alt="item.name" /></div>
    <div class="justify-center text-gray-50 flex h-[43px]">
        <div class="text-center leading-tight">{{item.name}}</div>
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
