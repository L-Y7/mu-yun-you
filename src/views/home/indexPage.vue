<script setup>
import { defineAsyncComponent } from 'vue'
import { Icon } from '@iconify/vue'
const HeaderComp = defineAsyncComponent(() => import('./components/HeaderComp.vue'))
const AnotherComp = defineAsyncComponent(() => import('./components/anotherPage.vue'))
const MainComp = defineAsyncComponent(() => import('./components/mainPage.vue'))
const GridComp = defineAsyncComponent(() => import('./components/gridPage.vue'))
const BottomComp = defineAsyncComponent(() => import('./components/bottomPage.vue'))
</script>

<template>
  <div >
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
      <div class="Lnleft">
        <span class="inleft"></span>
      </div>
      <div class="Lnright">
        <span class="inright"></span>
      </div>
    </main>
    <AnotherComp></AnotherComp>
    <MainComp></MainComp>
    <GridComp></GridComp>
    <BottomComp></BottomComp>
  </div>
</template>

<style scoped>
.banner {
  height: 420px;
  position: relative;
}
.banner .imgOne {
  height: 420px;
  width: 100%;
  object-fit: cover;
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
  top: 0px;
  left: 316px;
  opacity: 0;
}
.inbox .item:hover .inbox2 {
  opacity: 1;
}
.Lnleft {
  width: 32px;
  height: 44px;
  background: rgba(28, 31, 33, 0.4);
  position: absolute;
  top: 50%;
  left: 45px;
}
.Lnleft .inleft {
  height: 16px;
  width: 16px;
  border-right: 2px solid #ebe6e6;
  border-bottom: 2px solid #ebe6e6;
  transform: rotate(129deg);
  margin-left: 10px;
  margin-top: 10px;
  position: absolute;
  top: 4px;
  left: 0;
}
.Lnright {
  width: 32px;
  height: 44px;
  background: rgba(28, 31, 33, 0.4);
  position: absolute;
  top: 50%;
  right: 45px;
}
.Lnright .inright {
  height: 16px;
  width: 16px;
  border-right: 2px solid #ebe6e6;
  border-bottom: 2px solid #ebe6e6;
  transform: rotate(-45deg);
  margin-left: 10px;
  margin-top: 10px;
  position: absolute;
  top: 4px;
  left: -6px;
}
</style>
