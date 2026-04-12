<script setup>
import { defineAsyncComponent } from 'vue'

const HeaderComp = defineAsyncComponent(() => import('./components/HeaderComp.vue'))
</script>

<template>
  <div><HeaderComp></HeaderComp></div>
</template>

<style scoped></style>
