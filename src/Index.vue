<template>
  <div id="app">
    <sp-table :thead="thead" :trows="trows"></sp-table>
  </div>
</template>

<script>
var spTable = require('./components/Table')

module.exports = {
  name: 'index',
  data: function () {
    return {
      thead: ['#', 'florin', 'cosmin', 'onciu'],
      trows: [{
        val: [1, 'Mark', 'Otto', '@mdo']
      }, {
        val: [2, 'Jacob', 'Thornton', '@fat']
      }, {
        val: [3, 'Mihai', 'Vasilache', '@mihai']
      }]
    }
  },
  components: {
    spTable: spTable
  }
}
</script>

<style>
#app {
  width: 800px;
  margin: 60px auto 0;
}
</style>