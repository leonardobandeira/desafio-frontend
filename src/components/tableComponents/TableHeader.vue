<template>
  <th>{{ texto }}</th>
</template>

<script>
export default {
  name: "TableHeader",
  props: {
    texto: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
th {
  font-weight: 600;
  font-size: 0.8em;
}
</style>