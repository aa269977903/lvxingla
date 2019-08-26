<template>
    <div class="outSide">111
      <br>
      <!--ref操作dom-->
      <div ref="getMsg" @click="getMsgClick">haha</div>
      <div>I am {{childNum1}}</div>
      <div>I am {{childNum2}}</div>
      <br>
      <ref1 @something="something1"></ref1>
      <ref1 @something="something2"></ref1>
      <div>{{total}}</div>
    </div>
</template>

<script>
import Ref1 from './components/refTransferValue/Ref1'
export default {
  name: 'List',
  components: {Ref1},
  data () {
    return {
      childNum1: 0,
      childNum2: 0
    }
  },
  methods: {
    getMsgClick () {
      alert(this.$refs.getMsg.innerHTML)
    },
    something1 (msg) {
      this.childNum1 = msg
    },
    something2 (msg) {
      this.childNum2 = msg
    }
  },
  computed: {
    total: {
      get: function () {
        return this.childNum1 + this.childNum2
      }
    }
  }
}
</script>

<style scoped lang="stylus">
  .outSide
    font-size: 1rem
</style>
