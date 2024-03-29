<template>
  <div id="app" :class="[AppSetting.ready ? 'ready' : '']">
    <AppHeader />
    <main class="main">
      <div class="container">
        <ProductCard />
      </div>
    </main>
    <footer class="footer">
      <div class="container">
        <p class="light">I'm footer</p>
        <p class="semi-bold">YouTube</p>
      </div>
    </footer>
  </div>
</template>

<script setup>
import ProductCard from '@/components/ProductCard.vue'
import AppHeader from '@/components/Header/AppHeader.vue'
import { ref, onMounted } from 'vue'

const AppSetting = ref({
  ready: false
})

const downloadApp = onMounted(() => {
  document.onreadystatechange = () => {
    if (document.readyState == 'complete') {
      AppSetting.value.ready = true
    }
  }
})
</script>

<style lang="scss" scoped></style>
