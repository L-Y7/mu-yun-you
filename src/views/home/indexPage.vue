<script setup>
import { defineAsyncComponent } from 'vue'
import { Icon } from '@iconify/vue'
const HeaderComp = defineAsyncComponent(() => import('./components/HeaderComp.vue'))
</script>

<template>
  <div>
    <HeaderComp> </HeaderComp>
    <main class="banner">
      <img src="../../assets/images/banner1.jpg" class="imgOne" />
      <div class="inbox">
        <div class="item" v-for="item in 6" :key="item">
          <Icon icon="glyphs:plane-bold" class="plane" />

          <div>
            <div class="inboxd">热门出发地</div>
            <ul class="inboxul">
              <li>北京</li>
              <li>北京</li>
              <li>北京</li>
              <li>北京</li>
              <li>北京</li>
              <li>北京</li>
            </ul>
          </div>
          <span class="tou2"></span>
          <div class="inbox2">
            这是一大段内容
            这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容这是一大段内容
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<style scoped>
.banner {
  height: 420px;
  position: relative;
}
.banner .imgOne {
  height: 420px;
}
.banner .inbox {
  height: 420px;
  background: rgba(28, 31, 33, 0.4);
  width: 296px;
  position: absolute;
  top: 0;
  left: 90px;
  color: #ffffff;
  padding-left: 20px;
  overflow: hidden;
}
.inbox .inboxd {
  font-family: PingFangSC-Regular;
  font-size: 18px;
  color: #ffffff;
  text-align: justify;
  line-height: 26px;
  display: flex;
  align-items: center;
}

.inbox .inboxul {
  display: flex;
  font-family: PingFangSC-Regular;
  font-size: 14px;
  text-align: justify;
  line-height: 22px;
  gap: 10px;
}
.inbox .item {
  display: flex;
  align-items: center;
  margin-top: 20px;
  position: relative;

}
.inbox .item .plane {
  width: 32px;
  height: 32px;
  margin-right: 10px;
}
.inbox .item .tou2 {
  height: 6px;
  width: 6px;
  border-right: 2px solid #eee8e8;
  border-bottom: 2px solid #ebe6e6;
  transform: rotate(320deg);
  margin-left: 10px;
  margin-top: 10px;

}
.banner .inbox2 {
  height: 420px;
  background: rgba(28, 31, 33, 0.4);
  width: 296px;
  position: absolute;
  top: 0;
  left: 405px;
  opacity: 0;
}
.item:hover .inbox2 {
  opacity: 1;
}
</style>
