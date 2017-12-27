<template>
  <div id="fruits-list">
    <h1>Fruits Name</h1>
    <ul>
      <li v-for="fruit in fruits">
        {{ fruit.name }}
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    props: ['fruits']
  }
</script>

<style>

</style>
