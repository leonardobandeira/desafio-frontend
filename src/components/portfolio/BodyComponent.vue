<template>
  <div class="row content__tabela">
    <HeaderComponent>
      <template #left>
        <Title tipo="secondary" texto="Carteiras" />
      </template>
      <template #right>
        <Button tipo="buscar" texto="Exportar CSV" acao="exportar" />
      </template>
    </HeaderComponent>
    <br />
    <Table />
    <Linha />
  </div>
</template>

<script>
import HeaderComponent from "./HeaderComponent";

import Title from "./../form/Title";
import Button from "./../form/Button";
import Table from "./../form/Table";
import Linha from "./../Linha";
export default {
  name: "BodyComponent",
  components: {
    HeaderComponent,

    Title,
    Button,

    Table,

    Linha,
  },
};
</script>

<style>
</style>