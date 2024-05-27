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
    <div class="row content__tabela">
      slkanalcasslkanalcasslkanalcasslkanalcassl
      kanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkan
      alcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcas
    </div>
  </div>
</template>

<script>
import HeaderComponent from "./../components/portfolio/HeaderComponent";
import FilterComponent from "./../components/portfolio/FilterComponent";

import Title from "./../components/form/Title";
import Button from "./../components/form/Button";
export default {
  name: "Content",
  components: {
    HeaderComponent,
    FilterComponent,
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

.content__tabela {
  background: #fff;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.1);
  border-radius: 4px;
  justify-content: left;
  padding: 1.5em 0.5em;
  background: red;
}
</style>