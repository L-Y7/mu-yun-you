<script setup>
import { defineAsyncComponent } from 'vue'

const IndexPage = defineAsyncComponent(() => import('@/views/home/indexPage.vue'))
</script>

<template>
  <IndexPage></IndexPage>
</template>

<style></style>
