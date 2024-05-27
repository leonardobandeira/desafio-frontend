<template>
  <div id="app">
    <HeaderComponent>
      <template #left>
        <Logo :imagem="require('@/assets/logo.png')" />
      </template>
      <template #right>
        <Usuario usuario="Otávio Oliveira" />
      </template>
    </HeaderComponent>
    <Content />
    <Footer />
  </div>
</template>


<script>
import HeaderComponent from "./layouts/Header";
import Content from "./layouts/Content";
import Footer from "./layouts/Footer";

import Logo from './components/Logo'
import Usuario from './components/Usuario'

export default {
  name: "App",
  components: {
    HeaderComponent,
    Content,
    Footer,
    Logo,
    Usuario,
  },
};
</script>

<style>
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
  display: grid;
  grid-template-rows: 4em 1fr 6em;
  grid-auto-columns: ifr;
  grid-template-areas: "header" "content" "footer";
}

.header {
  grid-area: header;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
  background-color: #fff; /*f8f8f8 Exemplo de cor de fundo */
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
