<template>
  <td><slot></slot></td>
</template>

<script>
export default {
  name: "TableCell",
};
</script>

<style>
td {
  font-weight: 400;
  font-size: 0.8em;
}
</style>
