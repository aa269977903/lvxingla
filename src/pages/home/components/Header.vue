<template>
    <div class="header">
      <div class="head-left">返回</div>
      <div class="head-middle">
        <span class="iconfont">&#xe632;</span>
        输入城市/景点/游玩主题
      </div>
      <div class="head-rigth">城市3</div>
    </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="stylus" scoped>
  .header
    display flex
    height .86rem
    background #00bcd4
    color #fff
    .head-left
      width: .64rem
      float: left
      .back-icon
        text-align: center
        font-size: .4rem
    .head-middle
      flex 1
      height: .64rem
      line-height: .64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
    .head-rigth
      min-width: 1.04rem
      padding: 0 .1rem
      float: right
      text-align: center
      color: #fff
      .arrow-icon
        margin-left: -.04rem
        font-size: .24rem
</style>
