<template>
  <div class="btn" @click="discountPrice">DISCOUNT PRICE</div>
</template>

<script>
  export default {
    methods: {
      discountPrice() {
        this.$store.dispatch('discountPrice', {
          discountRate: 20
        });
      }
    }
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
