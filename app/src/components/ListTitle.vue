<template>
    <div>
        <h3>{{title}}
            <span class="badge rounded-pill bg-primary">{{lists}}</span>
        </h3>
    </div>
</template>

<script>
    export default {
        name : "ListTitle",
        props : {
            title: String,
            lists : Number
        }

    }
</script>

<style lang="scss" scoped>

</style>