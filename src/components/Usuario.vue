<template>
  <div class="usuario">
    <i class="far fa-user-circle icone__user"></i> <span>{{ usuario }}</span><i class="fa-solid fa-right-from-bracket icone__exit"></i>
  </div>
</template>

<script>
export default {
  name: "Usuario",
  props: {
    usuario: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.usuario {
  display: flex;
  align-items: center;
  padding: 0 10px;
}

.icone__user{
  font-size: 2em;
  padding-right: 0.2em;
}

.icone__exit{
  font-size: 1em;
  padding-left: 1em;
}
</style>
