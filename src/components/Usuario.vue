<template>
  <div class="usuario">
    <i class="fa-solid fa-user"></i> <span>{{ usuario }}</span>
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
</style>
