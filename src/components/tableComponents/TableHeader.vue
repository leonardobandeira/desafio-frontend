<template>
  <th><slot></slot></th>
</template>

<script>
export default {
  name: "TableHeader",
};
</script>

<style>
th {
  font-weight: 600;
  font-size: 0.8em;
}
</style>