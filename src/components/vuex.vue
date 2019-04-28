<template>
    <div>
      vuex {{$store.state.count}}
      <button type="button" @click="increment">+</button>
      <button type="button" @click="decrement">-</button>
    </div>
</template>

<script>
import { mapActions } from 'vuex'
export default {
  name: 'vuex',
  methods: mapActions([
    'increment',
    'decrement'
  ])
}
</script>

<style scoped>

</style>
