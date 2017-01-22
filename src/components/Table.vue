<template>
  <table class="table table-bordered">
    <table-head :thead="thead"/>
    <table-body :trows="trows"/>
  </table>
</template>

<script>
var TableHead = require('./Thead')
var TableBody = require('./TableBody')

module.exports = {
  name: 'sp-table',
  props: ['thead', 'trows'],
  components: {
    TableHead: TableHead,
    TableBody: TableBody
  }
}
</script>