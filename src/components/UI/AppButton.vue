<template>
  <div>
    <button class="button"><slot></slot></button>
  </div>
</template>

<script setup></script>

<style scoped>
.blue {
  .button {
    background-color: #1551e5;
    border-radius: 8px;
    color: #fff;
    height: 100%;
    width: 100%;


  }

  .button:hover {
    transition: 0.3s all;
    background-color: rgba(21, 81, 229, 0.44);
  }
}
.light-blue {

  .button {
    background-color: #f2f6ff;
    border-radius: 8px;
    color: #1551e5;
    height: 100%;
    width: 100%;
  }
}
.pro {
  .button {
    font-family: 'Gotham-pro';
  }
}
</style>
