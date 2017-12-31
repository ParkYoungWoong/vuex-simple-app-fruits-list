<template>
  <div class="btn">{{ btnName }}</div>
</template>

<script>
  export default {
    props: ['btnName']
  }
</script>

<style scoped>
  .btn {
    max-width: 700px;
    margin: 10px auto;
    padding: 10px 0;
    color: white;
    text-align: center;
    background: salmon;
    border-radius: 6px;
    cursor: pointer;
  }
</style>
