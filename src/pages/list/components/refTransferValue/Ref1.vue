<template>
  <div @click="handleClick">{{number}}</div>
</template>

<script>
export default {
  name: 'Ref1',
  data () {
    return {
      number: 0
    }
  },
  methods: {
    handleClick () {
      this.number++
      this.$emit('something', this.number)
    }
  }
}
</script>

<style scoped>

</style>
