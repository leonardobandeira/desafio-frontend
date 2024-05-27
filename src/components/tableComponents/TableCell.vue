<template>
  <td>{{ texto }}</td>
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
td {
  font-weight: 400;
  font-size: 0.8em;
}
</style>