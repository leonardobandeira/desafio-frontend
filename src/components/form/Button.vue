<template>
  <button :class="tipo" @click="acao">{{ texto }}</button>
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
.add {
  color: #fff;
  font-weight: 400;
  font-size: 1em;
  background-color: #007bff;
  padding: 0.4em 1em;
  border: #007bff;
  border-radius: 4px;
}

.btn__buscar {
  background: #fff;
  border: solid 0.12em #007bff;
  font-size: 1em;
  width: 7em;
  height: 2.4em;
  border-radius: 6px;
  color: #007bff;
}

.icon__buscar {
  padding-right: 1em;
}
</style>