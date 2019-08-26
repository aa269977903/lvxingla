<template>
  <div>
    <tr>
      <td>{{content}}</td>
    </tr>
    <br>
    <!--  ref 获取dom元素-->
    <div ref='hello' @click="handleClick">haha</div>

  </div>
</template>

<script>
export default {
  name: 'Table',
  data: function () {
    return {
      content: 'this is a row'
    }
  },
  methods: {
    handleClick: function () {
      alert(this.$refs.hello.innerHTML)
    }
  }
}
</script>

<style scoped>

</style>
