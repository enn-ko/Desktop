<template>
  <div class="p-3">
    <ListTitle title="List Uits" :lists="total"/>
    <ul class="list-group">
     <FruitList v-for="(list,index) in lists" :key="index" @toParent="run" :current-Index="index" :listtext="list"></FruitList>
    </ul>
  </div>
</template>

<script>
import ListTitle from "@/components/ListTitle.vue"
import FruitList from "./components/FruitList.vue";
  export default {
    name : "App",
    components : { ListTitle, FruitList },
    data() {
      return {
        lists: ['orange','mango','banana']
      }
    },
   computed: {
    total() {
      return this.lists.length 
    }
   },
    methods: {
      run(x) {
        this.lists.splice(x,1)
      }
    },
  }
</script>

<style lang="scss" scoped>

</style>