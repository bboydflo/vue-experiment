<template>
  <thead>
    <tr>
      <th v-for="name in thead" v-bind:florin="name">{{name}}</th>
      <th v-if="hasRemovable">has removable</th>
    </tr>
  </thead>
</template>

<script>
module.exports = {
  name: 'table-head',
  props: ['thead'],
  data: function () {
    return {
      hasRemovable: false
    }
  },
  created: function () {
    if (this.thead.length > 6) {
      // update has removable
      this.hasRemovable = true
    }
    console.log(this.thead)
  }
}
</script>