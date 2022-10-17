<template>
    <div>
        <li class="list-group-item w-25">{{listtext}}
            <button class="btn btn-sm btn-outline-danger" @click="addrun">Del</button>
        </li>
    </div>
</template>

<script>
    export default {
        name : "FruitList",
        props : ['listtext','currentIndex'],
        methods: {
            addrun() {
               this.$emit('toParent',this.currentIndex )
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>