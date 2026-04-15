<script setup>
import { defineAsyncComponent } from 'vue'

const CCard = defineAsyncComponent(() => import('./CCard.vue'))
const GreenCard = defineAsyncComponent(() => import('./GreenCard.vue'))
const CHeader = defineAsyncComponent(() => import('./CHeader.vue'))
</script>
<template>
  <div class="biggest">
    <CHeader></CHeader>

    <div class="biggest-box">
      <div>
        <img
          src="../../../../assets/images/jjzyx1.png"
          alt=""
          width="560px"
          height="270px"
          style="display: block"
        />

        <div style="display: flex; justify-content: space-between">
          <CCard></CCard>
          <CCard></CCard>
        </div>
      </div>

      <div style="display: flex; flex-wrap: wrap; justify-content: space-around">
        <CCard></CCard>
        <CCard></CCard>
        <CCard></CCard>
        <GreenCard></GreenCard>
      </div>
    </div>
  </div>
</template>

<style scoped>
.biggest {
  width: 1152px;
  margin: 0 auto;
}

.biggest-box {
  display: flex;
  justify-content: space-between;
}
</style>
