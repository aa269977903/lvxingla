<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Recommend',
  props: {
    recommendList: Array
  },
  data () {
    return {
      recommendList1: [
        {
          id: '001',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1504/47/4730a0c01664b63d.water.jpg_200x200_d7f52253.jpg',
          title: '武汉海昌极地海底公园222222222222222222sssssssssssssssssssssssssssssssssssss22',
          desc: '浪漫的海底公园2222222222222222222ssssssssssssssssss222'
        },
        {
          id: '002',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1501/f8/f8413365ed3e77ab.water.jpg_200x200_db81bbda.jpg',
          title: '木兰草原',
          desc: '青青草原'
        },
        {
          id: '003',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1504/89/892ea25a5d7d77cd.water.jpg_200x200_1760e424.jpg',
          title: '胜天农庄',
          desc: '田园生活'
        },
        {
          id: '004',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1501/bf/bf53a52a9e1c9905.water.jpg_200x200_01729033.jpg',
          title: '东湖海洋世界',
          desc: '鱼儿水里游'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height: .6rem
    background: #eeeeee
    text-indent: .2rem
  .item
    overflow hidden
    display flex
    height 1.9rem
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-button
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
</style>
