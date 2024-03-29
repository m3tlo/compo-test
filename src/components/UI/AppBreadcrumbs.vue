<template>
  <div>
    <menu class="breadcrumbs">
      <!-- <li v-for="item in items"  class="breadcrumbs-item">{{ item }}</li> -->
      <li class="breadcrumbs__item">Каталог</li>
      <li class="breadcrumbs__item">Обувь</li>
      <li class="breadcrumbs__item">Кроссовки</li>
      <li class="breadcrumbs__item">Беговые</li>
    </menu>
  </div>
</template>

<script setup></script>

<style scoped>
.breadcrumbs {
  display: flex;
  align-items: flex-start;
  min-height: 50px;

  gap: 18px;
  .breadcrumbs__item {
    position: relative;
    list-style: none;
    font-weight: 400;
    color: #828ead;
    font-size: 12px;
    cursor: pointer;
  }
  .breadcrumbs__item::before {
    position: absolute;
    content: '/';
    left: -12px;
  }
  .breadcrumbs__item:first-child::before {
    content: '';
  }
}
</style>
