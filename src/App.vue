<template>
  <div>
    <LikeHeader v-slot="slotProps">
        <h3>初めまして</h3>
        <p>{{ slotProps}}</p>
    </LikeHeader>
    <LikeNumber :total-number="number" @my-click="increment"></LikeNumber>
    <LikeNumber :total-number="number"></LikeNumber>
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

