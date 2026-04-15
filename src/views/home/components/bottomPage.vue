<script setup></script>
<template>
  <div class="center-wrap">
    <div class="top">
      <ul class="topone">
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行<span class="fenge"></span></li>
        <li>机酒自由行</li>
      </ul>
    </div>
    <div class="mid">
      <div class="ml">
        <div class="mlone icon"><div class="youzi">这是一段子</div></div>

        <div class="mltwo icon"><div class="youzi2">这是一段子</div></div>

        <div class="mlthree icon"><div class="youzi3">这是一段子</div></div>
      </div>
      <div class="mr"></div>
    </div>
  </div>
  <div class="bottom">
    <div class="center-wrap">
      <h1 class="bh">慕云游商城</h1>
    </div>
  </div>
</template>
<style scoped>
.center-wrap {
  position: relative;
}
.top .topone {
  display: flex;
  position: absolute;
  top: 130px;
  left: 0;
  font-family: PingFangSC-Regular;
  font-size: 18px;
  color: #1c1f21;
  line-height: 28px;
  gap: 30px;
}
.top .topone li {
  position: relative;
}
.topone li:not(:last-child)::after {
  content: '';
  width: 2px;
  height: 15px;
  background: #161718;
  position: absolute;
  right: -15px;
  top: 50%;
  transform: translateY(-50%);
}
.ml {
  position: absolute;
  top: 180px;
  left: -150px;
  height: 200px;
  width: 100%;
  display: flex;
  justify-content: space-around;
}
.icon {
  background-image: url('../../../assets/images/icons.png');
  background-repeat: no-repeat;
  display: inline-block;
}
.mlone {
  position: relative;
  width: 60px;
  height: 60px;
  background-position: -150px -31px;
}
.mltwo {
  position: relative;
  width: 60px;
  height: 60px;
  background-position: -150px -104px;
}
.mlthree {
  position: relative;
  width: 60px;
  height: 60px;
  background-position: -150px -178px;
}

.youzi {
  position: absolute;
  top: 50%;
  left: 60px;
  width: 90px;
  height: 90px;
}
.youzi2 {
  position: absolute;
  top: 50%;
  left: 60px;
  width: 90px;
  height: 90px;
}
.youzi3 {
  position: absolute;
  top: 50%;
  left: 60px;
  width: 90px;
  height: 90px;
}
.bottom {
  height: 225px;
  background: #1c1f21;
  width: 100%;
  position: absolute;
  bottom: -1600px;
  color: #ffffff;
}
.bh {
  font-family: PingFangSC-Regular;
  font-size: 46px;
  color: #ffffff;
  line-height: 46px;
  margin-top: 30px;
}
</style>
