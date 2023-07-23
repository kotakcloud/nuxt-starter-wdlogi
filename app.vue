<template>
  <div class="container">
    <Button @click="increaseCount" label="Count"></Button>
    <h5 class="green">{{ count }}</h5>
  </div>
</template>

<script setup lang="ts">
const count = ref(0);

const increaseCount = () => {
  count.value++;
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
