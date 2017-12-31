<template>
  <div id="app">
    <h1 id="app-title">Fruits List</h1>
    <div id="fruits-table">
      <fruits-list></fruits-list>
      <fruits-price></fruits-price>
    </div>
    <btn-component :btnName="'Discount'"></btn-component>
  </div>
</template>

<script>
import FruitsList from './components/FruitsList.vue';
import FruitsPrice from './components/FruitsPrice.vue';
import BtnComponent from './components/Btn.vue';

export default {
  name: 'app',
  data () {
    return {

    }
  },
  components: {
    'fruits-list': FruitsList,
    'fruits-price': FruitsPrice,
    'btn-component': BtnComponent
  }
}
</script>

<style>
  @import url("css/app.css");
</style>
