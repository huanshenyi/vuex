<template>
    <div class="a">
      page a{{this.$store.state.money.money}}
      <button @click="add" type="button">+</button>
      <button @click="reduce" type="button">-</button>
    </div>

</template>

<script>
  import { mapActions } from 'vuex'
  export default {
    name: 'pagea',
    methods: mapActions('money', ['add', 'reduce'])
  }
</script>

<style scoped>

</style>
