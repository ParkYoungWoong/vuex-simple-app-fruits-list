<template>
  <div id="fruits-list">
    <h1>Fruits Name</h1>
    <ul>
      <li v-for="fruit in upperCaseFruits">
        {{ fruit.name }}
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    computed: {
      fruits() {
        return this.$store.state.fruits;
      },
      upperCaseFruits() {
        return this.$store.getters.upperCaseFruits;
      }
    }
  }
</script>

<style></style>
