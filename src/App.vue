<template>
  <div>
    <LikeHeader>
        <template v-slot:title>
          <h2>こんにちは</h2>
        </template>
        <h3>初めましてっ</h3>
        <template v-slot:number>
          <p>{{ number }}</p>
        </template>
    </LikeHeader>
  </div>
</template>

<script>
import LikeHeader from './components/LikeHeader'

export default {
  data() {
    return {
      number:14
    }
  },
  components: {
    LikeHeader
  },
  methods: {
    increment() {
      this.number++
    }
  }
}
</script>

<style scoped>
  div {
    border: 1px solid blue
  }
</style>

