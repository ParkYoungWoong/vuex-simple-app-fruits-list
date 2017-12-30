<template>
  <div id="fruits-price">
    <h1>Fruits Price</h1>
    <ul>
      <li v-for="fruit in fruits">
        $ {{ fruit.price }}
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    computed: {
      fruits() {
        return this.$store.state.fruits
      }
    }
  }
</script>

<style></style>
