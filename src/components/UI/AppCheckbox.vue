<template>
  <label >
    <div :class='["v-checkbox", checkboxSetting.active ? "active" : "" ]'><span class='v-checkbox__ball'></span></div>
    <input class='checkbox' type='checkbox' v-model='checkboxSetting.active'>
    <span> <slot></slot></span>
  </label>
</template>

<script setup>
  import {ref} from 'vue'

  const checkboxSetting = ref({
    active: false,
  })
</script>

<style scoped>
.v-checkbox{
  cursor: pointer;
  box-sizing: border-box;
  padding: 2px;
  position: relative;
  width: 40px;
  height: 24px;
  border-radius: 32px;
  background:#828EAD;
  .v-checkbox__ball{
    display: inline-block;
    width: 20px;
    height: 20px;
    position: absolute;
    border-radius: 50%;
    margin-right:  16px;

    background: #fff;
    transition: all .3s;

  }
}
.v-checkbox.active{
  background: #1551E5;
  .v-checkbox__ball{
    transition: all .3s;
  margin-left: 16px;
  }
}
.checkbox{
display: none;
}
label{
  display: flex;
  align-items: center;
  gap: 12px;
}
</style>
