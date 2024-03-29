<template>
  <nav class="header__nav-container">
    <div class="container">
      <menu class="header__menu">
        <li class="header__menu-item"><a href="#" class="pro">Мои заказы</a></li>
        <li class="header__menu-item"><a href="#" class="pro">Сотрудники</a></li>
        <li class="header__menu-item"><a href="#" class="pro">Шаблоны заказов</a></li>
        <li class="header__menu-item"><a href="#" class="pro">Обращение</a></li>
      </menu>
      <div @click="showMenu" class="header__menu-additional-info">
        <AppButton class="light-blue pro">Ваш менеджер</AppButton>
        <a href="#" class="pro blue">% Акции</a>
        <a href="#" class="pro blue">Блог</a>
      </div>
    </div>
  </nav>
</template>
<script setup>
import AppButton from '@/components/UI/AppButton.vue'
</script>

<style scoped>
.header__nav-container {
  * {
    flex-shrink: 1;
  }
}
</style>
