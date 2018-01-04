<template>
  <div class="btn" @click="price(discountData)">DISCOUNT PRICE</div>
</template>

<script>
  import { mapActions } from 'vuex';

  export default {
    data() {
      return {
        discountData: {
          rate: 20
        }
      }
    },
    methods: {
      ...mapActions({
        price: 'discountPrice'
      })
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
