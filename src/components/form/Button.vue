<template>
  <button :class="tipo" @click="acao">
    <i v-if="icone" :class="`fa-solid ${icone}`"></i>

    {{ texto }}
  </button>
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
      type: Function,
      required: true,
    },
    icone: {
      type: String,
    },
  },
};
</script>

<style>
.adicionar {
  color: #fff;
  font-size: 1em;
  font-weight: 400;
  height: 2.7em;
  background-color: #007bff;
  padding: 0.4em 1.8em;
  border: #007bff;
  border-radius: 4px;
  cursor: pointer;
}

.buscar {
  background: #fff;
  border: solid 0.12em #007bff;
  font-size: 1em;
  font-weight: 400;
  height: 2.7em;
  border-radius: 2px;
  color: #007bff;
  cursor: pointer;
}

.buscar i {
  padding-right: 0.4em;
}
</style>