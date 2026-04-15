<script setup></script>
<template>
  <div class="c-header">
    <div class="left">
      <div class="tf">机酒自由行</div>
    </div>
    <div class="right">
      <ul class="ur">
        <li><a href="#">近期好货</a></li>
        <li><a href="#">近期好货</a></li>
        <li><a href="#">近期好A货</a></li>
        <li><a href="#">近期好货</a></li>
        <li><a href="#">近期好货</a></li>
        <li><a href="#">近期好货</a></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.c-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.c-header .tf {
  font-family: PingFangSC-Medium;
  font-size: 36px;
  color: #000000;
  text-align: justify;
  line-height: 54px;
  margin-top: 30px;
  margin-bottom: 30px;
}
.right .ur {
  display: flex;
  gap: 10px;
}
.right .ur a {
  color: #131413;
  display: block;
}
.right .ur a:hover {
  color: #15af7a;
  color: #15af7a;
  /* border-bottom: 2px solid #15af7a; */
  box-shadow: 0 6px 8px -6px rgba(21, 175, 122, 0.5);
}
</style>
