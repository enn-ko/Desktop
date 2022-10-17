<template>
  <div class="hello card mt-3 shadow-sm w-50 p-3 text-center">
    <h4>{{ msg }}</h4>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
