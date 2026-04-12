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
              <li>社区</li>
            </a>
            <a href="#" class="lianjie">
              <li>行程助手</li>
            </a>
            <a href="#" class="lianjie">
              <li>商城</li>
            </a>
            <a href="#" class="lianjie">
              <li>酒店·民宿</li>
            </a>
            <a href="#" class="lianjie">
              <li>特价酒店</li>
            </a>
          </ul>
        </div>
        <div class="rightOne">
          <Icon icon="mdi-light:home" />
          <div class="xian"></div>
          <Icon icon="mdi-light:home" />
          <Icon icon="ic:baseline-wechat" />

          <div>登录</div>
          <div>注册</div>
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

.center-wrap {
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
</style>
