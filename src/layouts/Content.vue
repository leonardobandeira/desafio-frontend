<template>
  <div class="content">
    <HeaderComponent>
      <template #left>
        <Title tipo="primary" texto="BTC Carteiras" />
      </template>
      <template #right>
        <Button tipo="adicionar" texto="Adicionar Carteira" acao="add" />
      </template>
    </HeaderComponent>

    <FilterComponent />
    <BodyComponent />
  </div>
</template>

<script>
import HeaderComponent from "./Header";
import FilterComponent from "./../components/portfolio/FilterComponent";
import BodyComponent from "./../components/portfolio/BodyComponent";

import Title from "./../components/form/Title";
import Button from "./../components/form/Button";
export default {
  name: "Content",
  components: {
    HeaderComponent,
    FilterComponent,
    BodyComponent,

    Title,
    Button,
  },
};
</script>

<style>
.content {
  grid-area: content;
  padding: 3em 10em 0 10em;
  background-color: #f8f8f8;
}
</style>