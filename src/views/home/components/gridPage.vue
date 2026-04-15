<script setup>
import { Icon } from '@iconify/vue'
</script>
<template>
  <div class="biggest">
    <div class="center-wrap">
      <div class="top">
        <div class="left">
          <div class="tf">机酒自由行</div>
        </div>
        <div class="right">
          <ul class="ur">
            <li><a href="#">近期好货</a></li>
            <li><a href="#">近期好货</a></li>
            <li><a href="#">近期好货</a></li>
            <li><a href="#">近期好货</a></li>
            <li><a href="#">近期好货</a></li>
            <li><a href="#">近期好货</a></li>
          </ul>
        </div>
      </div>
      <div class="bottom">
        <!-- <div class="pubu">
          <img src="../../../assets/images/jjzyx2.png" />
          <img src="../../../assets/images/jjzyx3.png" />
          <img src="../../../assets/images/jjzyx4.png" />
          <img src="../../../assets/images/jjzyx5.png" />
          <img src="../../../assets/images/jjzyx6.png" /> -->
        <div class="pubu">
          <div class="item big">
            <img src="../../../assets/images/jjzyx1.png" />
            <div class="cover">
              <span class="fangzhi">机票</span>
              <div class="tanchu">可以去的地方</div>
            </div>
          </div>
          <div class="item">
            <img src="../../../assets/images/jjzyx2.png" />
            <div class="cover">
              <span class="fangzhi">机票</span>
              <div class="tanchu">可以去的地方</div>
            </div>
          </div>
          <div class="item">
            <img src="../../../assets/images/jjzyx3.png" />
            <div class="cover">
              <span class="fangzhi">机票</span>
              <div class="tanchu">可以去的地方</div>
            </div>
          </div>
          <div class="item">
            <img src="../../../assets/images/jjzyx4.png" />
            <div class="cover">
              <span class="fangzhi">机票</span>
              <div class="tanchu">可以去的地方</div>
            </div>
            <span class="cover3">这是一大段描述的话</span>
          </div>
          <div class="item">
            <img src="../../../assets/images/jjzyx5.png" />
            <div class="cover">
              <span class="fangzhi">机票</span>
              <div class="tanchu">可以去的地方</div>
            </div>
            <span class="cover3">这是一大段描述的话</span>
          </div>
          <div class="item">
            <img src="../../../assets/images/jjzyx6.png" />
            <div class="cover">
              <span class="fangzhi">机票</span>
              <div class="tanchu">可以去的地方</div>
            </div>
            <span class="cover3">这是一大段描述的话</span>
          </div>
          <div class="green">
            <div class="gone">机酒自由行产片</div>
            <div class="gtwo"><Icon icon="gg:arrow-right-o" /></div>
            <div class="gthree">机票<span class="fenge"></span>酒店</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.top {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.top .tf {
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
.bottom .pubu {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: 230px;
  gap: 20px;
  font-family: PingFangSC-Regular;
  font-size: 14px;
  color: #ffffff;
  text-align: center;
  line-height: 22px;
}
.bottom .pubu .item {
  position: relative;
}
.item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}
.pubu .big {
  grid-column: span 2;
}

.item .cover {
  position: absolute;
  bottom: 0;
  left: 0;
  opacity: 0.55;
  background: #1c1f21;
}
.cover .tanchu{
  display: none;
}
.cover:hover .tanchu{
 display: block;
}
.item .cover3 {
  background: #ffffff;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.08);
  color: #1c1f21;
  width: 273px;
  height: 43px;
  display: inline-block;
}
.green {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  height: 270px;
  width: 264px;
  background-image: linear-gradient(180deg, #34e3bc 0%, #15af7a 98%);
  box-shadow: 0 4px 8px 0;
}
.green .gtwo {
  font-size: 88px;
}
.green .gthree .fenge {
  display: inline-block;
  width: 2px;
  height: 12px;
  background: #fff;
  margin: 0 8px;
}
</style>
