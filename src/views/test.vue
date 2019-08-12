<template>
  <div class="test">
    <h1>{{message}}</h1>
    <van-swipe :autoplay="3000" :height="200" indicator-color="white">
      <van-swipe-item><div class="item">123</div></van-swipe-item>
      <van-swipe-item><div class="item">fds</div></van-swipe-item>
    </van-swipe>
  </div>
</template>

<script>
import { Swipe, SwipeItem } from 'vant';
import 'vant/lib/swipe/index.css';
import 'vant/lib/swipe-item/index.css';

export default {
  data() {
    return {
      message: 123,
    }
  },
  methods: {  
   
  },
  components: {
    vanSwipe: Swipe,
    vanSwipeItem: SwipeItem
  }
}
</script>

<style lang="scss">
  .van-swipe-item:nth-child(even) {
    background-color: #39a9ed;
  }
  .van-swipe-item:nth-child(odd) {
    background-color: red;
  }
</style>

