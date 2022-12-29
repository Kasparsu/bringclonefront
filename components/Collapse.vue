<template>
      <div :class="{'collapse-open': active}" class="collapse collapse-arrow border border-base-300 bg-base-100 rounded-box">
        <div @click="active=!active" class="collapse-title text-xl font-medium">
            {{title}}
        </div>
        <div class="collapse-content"> 
            <slot></slot>
        </div>
    </div>
</template>

<script>
export default {
    props: ['title'],
    data(){
        return {
            active: false,
        }
    }
}
</script>

<style>

</style>
