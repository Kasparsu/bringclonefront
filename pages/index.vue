<template>
  <div class="container mx-auto">
        <collapse v-for="category in categories" :key="category.id" :title="category.name">
            <div class="grid grid-cols-12 gap-1">
                <div v-for="item in category.items" :key="item.id" >
                    <item :item="item"></item>
                </div>
                
            </div>
        </collapse>
  </div>
</template>

<script>
import Collapse from '../components/Collapse.vue'
import axios from 'axios';
import Item from '../components/Item.vue';
export default {
  components: { Collapse, Item },
    created(){
        axios.get('http://localhost:8000/api/items').then(res => {
            this.categories = res.data;
        })
    },
    data(){
        return {
            categories: []
        }
    }
}
</script>

<style>

</style>