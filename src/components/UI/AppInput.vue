<template>
  <div>
    <input :placeholder="placeholder" type="text" class="input" />
    <div class="buttons">
      <button type="reset " class="pro-light">
        <i class="fi fi-rr-cross" style="font-size: 15px"></i>
      </button>
      <button type="submit " class="pro-light"><i class="fi fi-rr-search"></i></button>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.search {
  position: relative;
  display: flex;
  min-width: 45%;
  .input {
    border: 1px solid #e1e5eb;
    border-right: none;
    border-radius: 8px;
    min-height: 48px;
    min-width: 100%;
    padding: 15px;
    box-sizing: border-box;
  }
  .input:focus-visible,
  .input:focus {
    outline: 2px solid #1551e5;
  }
  .input:hover {
    border: 1px solid #828ead;
  }
  .buttons {
    display: flex;
    gap: 10px;
    position: absolute;
    border-right: 1px solid #e1e5eb;
    height: 48px;
    border-radius: 8px;
    right: 0;
    align-items: center;
    padding: 15px;
    box-sizing: border-box;
    .fi {
      font-size: 17px;
    }
  }
  button {
    font-weight: 400;
    border: none;
    cursor: pointer;
    background: none;
    padding: 5px;
  }
}

.search:has(.input:hover) {
  .buttons {
    border-right: 1px solid #828ead;
  }
}
</style>
