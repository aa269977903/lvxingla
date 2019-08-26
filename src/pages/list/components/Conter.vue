<template>
  <div @click="handleClick">{{content}}</div>
</template>

<script>
export default {
  name: 'Conter',
  data: function () {
    return {
      content: 0
    }
  },
  methods: {
    handleClick: function () {
      this.content++
      this.$emit('change1')
    }
  }
}
</script>

<style scoped>

</style>
