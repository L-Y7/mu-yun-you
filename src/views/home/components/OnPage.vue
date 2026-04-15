<script setup></script>
<template>
  <div class="big2">
    <div class="center-wrap">
      <div class="san">
        <div class="sanone">
          <img src="../../../assets/images/ddwl1.png" />
          <div>这是一段话</div>
        </div>
        <div class="sanone">
          <img src="../../../assets/images/ddwl2.png" />
          <div>这是一段话</div>
        </div>
      </div>
      <div class="san">
        <div class="sanone">
          <img src="../../../assets/images/ddwl3.png" />
          <div>这是一段话</div>
        </div>
        <div class="sanone">
          <img src="../../../assets/images/ddwl4.png" />
          <div>这是一段话</div>
        </div>

        <div class="sanone">
          <img src="../../../assets/images/ddwl5.png" />
          <div>这是一段话</div>
        </div>
      </div>
      <div class="san">
        <div class="sanone">
          <img src="../../../assets/images/ddwl6.png" />
          <div>这是一段话</div>
        </div>
        <div class="sanone">
          <div class="red"></div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.center-wrap {
  display: flex;
}
.big2 {
  height: 586px;
}
.san {
  display: flex;
  flex-direction: column;
  gap: 30px;
  align-items: flex-start;
}
.sanone {
  display: flex;
}

.sanone div {
  height: 30px;
}
.red {
  background-image: linear-gradient(180deg, #ff6374 1%, #ff7368 98%);
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.08);
  height: 370px;
  width: 360px;
  flex-shrink: 0;
}
</style>
