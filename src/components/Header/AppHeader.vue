<template>
  <header class="header">
    <div class="header__content-container">
      <div class="container">
        <AppLogo />
        <AppButton @click="changeShowMenu" class="blue pro">Меню</AppButton>
        <AppInput class="search" />
        <div class="header__icons">
          <i class="fi fi-rr-bell"></i>
          <i class="fi fi-rr-heart"></i>
        </div>
        <AppButton class="light-blue pro header">Корзина: 144 235₽</AppButton>
        <div class="header__user">
          <div class="user">
            <img src="@/assets/icons/Avatar.png" alt="user-avatar" class="user__photo" />
            <p class="user__name pro">Ермаков Е.</p>
          </div>
          <button class="button"><MenuArrow /></button>
        </div>
      </div>
    </div>
    <HeaderMenu :class="['hide', headerSetting.showMenu ? 'showed' : 'hidden']" />
  </header>
</template>

<script setup>
import AppInput from '@/components/UI/AppInput.vue'
import HeaderMenu from './HeaderMenu.vue'
import AppButton from '@/components/UI/AppButton.vue'
import MenuArrow from '@/components/icons/MenuArrow.vue'
import AppLogo from '@/components/icons/AppLogo.vue'

import { ref } from 'vue'

const headerSetting = ref({
  showMenu: false
})

const changeShowMenu = () => {
  if (!headerSetting.value.showMenu) {
    headerSetting.value.showMenu = true
  } else {
    headerSetting.value.showMenu = false
  }
}
</script>

<style>
@import url('./header.css');

div.blue {
  min-height: 48px;
  min-width: 5%;

  button.button {
    width: 100%;
    min-height: 48px;
    display: block;
  }
}
div.light-blue.header {
  min-height: 48px;
  button.button {
    width: 100%;
    min-height: 48px;
    display: block;
  }
}
.header__user {
  display: flex;
  .button {
    /* transform: rotate(90deg); */
    padding: 0;
  }
  .user {
    display: flex;
    align-items: center;
    gap: 16px;
  }
}
.header__icons {
  display: flex;
  align-items: center;
  font-size: 25px;
  .fi {
    height: 30px;
    padding: 0 10px;
  }
  .fi:last-child {
    border-left: 1px solid #e2e4f0;
  }
}
</style>
