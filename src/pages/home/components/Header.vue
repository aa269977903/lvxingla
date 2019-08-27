<template>
    <div class="header">
      <div class="head-left">
        <div class="iconfont back-icon">&#xe624;</div>
      </div>
      <div class="head-middle">
        <span class="iconfont">&#xe632;</span>
        输入城市/景点/游玩主题
      </div>
      <router-link to='/city'>
        <div class="head-rigth">
          {{this.$store.state.city}}
          <span class="iconfont arrow-icon">&#xe632;</span>
        </div>
      </router-link>
    </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display flex
    line-height  $headerHeight
    background $bgColor
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
