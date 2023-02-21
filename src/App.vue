<script setup>

</script>

<template>
  <div class="container"><h1>Tier list</h1>
    <div class="placeholder"><h2>S+</h2></div>
    <div class="placeholder"><h2>S</h2></div>
    <div class="placeholder"><h2>A</h2></div>
    <div class="placeholder"><h2>B</h2></div>
    <div class="placeholder"><h2>C</h2></div>
    <div class="placeholder"><h2>D</h2></div>
  
  </div>
</template>

<style scoped lang="scss">
.container {
  background-color: rgba(255, 255, 255, 0.1);
  width: 80vw;
  position: fixed;
  top: 5vh;
  left: 10vw;
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  
  h1 {
    text-align: center;
  }

  .placeholder {
    width: calc(100% - 40px);
    margin: 20px;
    height: 100px;
    background-color: rgba(255, 255, 255, 0.1);
    display: flex;

    h2 {
      height: 100%;
      aspect-ratio: 1 / 1;
      background-color: rgba(255, 255, 255, 0.1);
      margin: 0;
      text-align: center;
      line-height: 100px;
      font-size: 32px;
    }
  }
}
</style>
