<template>
  <div id="app">
    <h1 id="app-title">Fruits List</h1>
    <div id="fruits-table">
      <fruits-list></fruits-list>
      <fruits-price></fruits-price>
    </div>
  </div>
</template>

<script>
import FruitsList from './components/FruitsList.vue';
import FruitsPrice from './components/FruitsPrice.vue';

export default {
  name: 'app',
  data () {
    return {

    }
  },
  components: {
    'fruits-list': FruitsList,
    'fruits-price': FruitsPrice
  }
}
</script>

<style>
  @import url("css/app.css");
</style>
