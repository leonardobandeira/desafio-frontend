<template>
  <div class="row content__body">
    <HeaderComponent>
      <template #left>
        <Title tipo="secondary" texto="Carteiras" />
      </template>
      <template #right>
        <Button tipo="buscar" texto="Exportar CSV" acao="exportar" />
      </template>
    </HeaderComponent>
    <br />
    <Table>
    
    </Table>
    <Linha />
  </div>
</template>

<script>
import HeaderComponent from "./../../layouts/Header";

import Title from "./../form/Title";
import Button from "./../form/Button";
import Table from "./../tableComponents/Table";
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
.content__body {
  background: #fff;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.1);
  border-radius: 4px;
  justify-content: left;
  padding: 1.5em 0.5em;
}
</style>