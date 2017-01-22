<template>
  <tbody>
    <tr v-for="row in trows">
      <td v-for="v in row.val">{{v}}</td>
    </tr>
  </tbody>
</template>

<script>
export default {
  name: 'table-body',
  props: ['trows']
}
</script>