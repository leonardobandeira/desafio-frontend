<template>
  <span :class="tipo">{{ texto }}</span>
</template>

<script>
export default {
  name: "Title",
  props: {
    tipo: {
      type: String,
      required: true,
    },
    texto: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
.primary {
  color: #000;
  font-size: 1.5em;
  font-weight: 700;
}

.secondary {
  color: rgb(146, 155, 155);
  font-size: 1em;
  font-weight: 700;
}
</style>