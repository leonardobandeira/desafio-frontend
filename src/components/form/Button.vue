<template>
  <button class="btn__add__carteira" @click="acao">{{ texto }}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    tipo: {
      type: String,
      required: true,
    },
    texto: {
      type: String,
      required: true,
    },
    acao: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
.btn__add__carteira {
  color: #fff;
  font-weight: 400;
  font-size: 1em;
  background-color: #007bff;
  padding: 0.4em 1em;
  border: #007bff;
  border-radius: 4px;
}
</style>