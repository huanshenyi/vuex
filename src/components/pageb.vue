<template>
    <div class="b">
      page b{{$store.state.count.count}}
      <button @click="add(2)" type="button">+</button>
      <button @click="reduce" type="button">-</button>
    </div>
</template>

<script>
  import { mapActions } from 'vuex'
  export default {
    name: 'pageb',
    methods: mapActions('count', ['add', 'reduce'])
  }
</script>

<style scoped>

</style>
