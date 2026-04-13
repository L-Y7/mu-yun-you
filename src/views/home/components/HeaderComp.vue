<script setup>
import { Icon } from '@iconify/vue'
</script>

<template>
  <header class="site-head">
    <div class="topbar">
      <div class="center-wrap">
        <div class="leftOne">
          <ul class="ulOne">
            <a href="#" class="lianjie">
              <li>目的地</li>
            </a>
            <a href="#" class="lianjie">
              <li>锦囊</li>
            </a>
            <a href="#" class="lianjie">
              <li class="jian">
                社区
                <span class="tou"></span>
              </li>
            </a>
            <a href="#" class="lianjie">
              <li>行程助手</li>
            </a>
            <a href="#" class="lianjie">
              <li class="jian">
                商城
                <span class="tou"></span>
              </li>
            </a>
            <a href="#" class="lianjie">
              <li class="jian">酒店·民宿 <span class="tou"></span></li>
            </a>
            <a href="#" class="lianjie">
              <li>特价酒店</li>
            </a>
          </ul>
        </div>
        <div class="rightOne">
          <Icon icon="material-symbols:search" />
          <div class="xian"></div>
          <Icon icon="mdi-light:home" />
          <Icon icon="ic:baseline-wechat" />

          <div>登录</div>
          <div>注册</div>
        </div>
      </div>
    </div>
    <div class="topbarTwo">
      <div class="center-wrap">
        <ul class="ulTwo">
          <li class="cai">
            机酒自由行
            <span class="dan"></span>
          </li>
          <li>优惠机票</li>
          <li>跟团游</li>
          <li>酒店</li>
          <li>当地玩乐</li>
          <li>深度旅游</li>
        </ul>
      </div>
    </div>
    <div class="topbarThree">
      <div class="center-wrap">
        <h1>慕云游商城</h1>
        <div class="input-box">
          <input type="text" class="in" />
          <span class="green"> <Icon icon="material-symbols:search" class="g" /></span>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.site-head {
  height: 150px;
  color: aliceblue;
}
.topbar {
  background: #2a2a2a;
  height: 32px;
}
.topbar .ulOne {
  display: flex;
}

.topbar .ulOne .lianjie {
  color: aliceblue;
}

.topbar .ulOne li {
  line-height: 32px;
  margin-right: 20px;
}
.ulOne .jian {
  display: flex;
  align-items: center;
}
.ulOne .jian .tou {
  height: 6px;
  width: 6px;
  border-right: 2px solid #eee8e8;
  border-bottom: 2px solid #ebe6e6;
  transform: rotate(45deg);
  margin-left: 3px;
}

.topbar .center-wrap {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.center-wrap .rightOne {
  display: flex;
  align-items: center;
  gap: 10px;
}
.rightOne .xian {
  height: 15px;
  border-left: 2px solid white;
}
.topbarTwo {
  background: #20bd9a;
  height: 40px;
}
.topbarTwo .ulTwo {
  display: flex;
}
.topbarTwo .center-wrap .ulTwo {
  line-height: 40px;
  gap: 20px;
}
.ulTwo .cai {
  display: flex;
  align-items: center;
}
.ulTwo .cai .dan {
  width: 0;
  height: 0;
  border-left: 4px solid transparent;
  border-right: 4px solid transparent;
  border-top: 6px solid #ebe6e6;
  margin-left: 5px;
  margin-top: 2px;
}
.topbarThree {
  background: #ffffff;
  height: 78px;
}
.topbarThree .center-wrap {
  display: flex;
  align-items: center;
  height: 100%;
}
h1 {
  font-family: PingFangSC-Medium;
  font-size: 24px;
  color: #20bd9a;
  text-align: justify;
  line-height: 36px;
  margin-right: 30px;
}
.input-box {
  position: relative;
}
.input-box .in {
  opacity: 0.3;
  border: 1px solid #20bd9a;
  border-radius: 4px;
  width: 405px;
  height: 30px;
}
.input-box .green {
  position: absolute;
  right: 0;
  top: 0;
  width: 30px;
  height: 100%;
  background: #20bd9a;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
