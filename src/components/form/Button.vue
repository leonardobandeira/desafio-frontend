<template>
  <button :class="tipo" @click="acao">
    <i
      v-if="tipo === 'buscar'"
      class="fa-solid fa-magnifying-glass icon__buscar"
    ></i>
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
  },
};
</script>

<style>
.adicionar {
  color: #fff;
  font-size: 1.em;
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
  font-size: 1.em;
  font-weight: 400;
  height: 2.7em;
  border-radius: 2px;
  color: #007bff;
  cursor: pointer;

  i {
    padding-right: 0.4em;
  }
}
</style>