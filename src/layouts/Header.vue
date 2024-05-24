<!-- src/components/Header.vue -->
<template>
  <div class="header">
    <Logo :imagem="require('@/assets/logo.jpg')" />
    <Usuario usuario="Usuário" />
  </div>
</template>

<script>
import Logo from "./../components/Logo";
import Usuario from "./../components/Usuario";

export default {
  name: "Header",
  components: {
    Logo,
    Usuario,
  },
};
</script>

<style scoped>
.header {
  grid-area: header;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
  background-color: red; /*f8f8f8 Exemplo de cor de fundo */
}

.header h1 {
  margin: 0;
  flex: 1;
  text-align: center;
}

.menu-do-usuario {
  flex-shrink: 0;
}
</style>
