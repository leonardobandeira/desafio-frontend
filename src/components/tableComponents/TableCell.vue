<template>
  <td :width="tamanho"><slot></slot></td>
</template>

<script>
export default {
  name: "TableCell",
  props: {
    tamanho: {
      type: Number,
    },
  },
};
</script>

<style>
td {
  font-weight: 400;
  font-size: 0.8em;
}
</style>
