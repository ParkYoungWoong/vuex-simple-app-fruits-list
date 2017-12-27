<template>
  <div id="app">
    <h1 id="app-title">Fruits List</h1>
    <div id="fruits-table">
      <fruits-list :fruits="fruits"></fruits-list>
      <fruits-price :fruits="fruits"></fruits-price>
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
      fruits: [
        { name: 'Apple', price: 30 },
        { name: 'Banana', price: 40 },
        { name: 'Mango', price: 50 },
        { name: 'Orange', price: 60 },
        { name: 'Tomato', price: 70 },
        { name: 'Pineapple', price: 80 }
      ]
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
