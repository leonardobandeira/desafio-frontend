<template>
  <div class="row content__tabela">
    <HeaderComponent>
      <template #left>
        <Title tipo="secondary" texto="Carteiras" />
      </template>
      <template #right>
        <Button tipo="buscar" texto="Exportar CSV" :acao="openModal"/>
      </template>
    </HeaderComponent>
    <br />
    <Table> </Table>
    <Linha />

    <Modal :showModal="modalOpen" @close="closeModal">
     Preparando para exportar
    </Modal>
  </div>
</template>

<script>
import HeaderComponent from "./../../layouts/Header";

import Title from "./../form/Title";
import Button from "./../form/Button";
import Table from "./../tableComponents/Table";
import Linha from "./../Linha";
import Modal from "../Modal";

export default {
  name: "BodyComponent",
  components: {
    HeaderComponent,

    Title,
    Button,

    Table,

    Linha,
    Modal,
  },
  data() {
    return {
      modalOpen: false,
    };
  },
  methods: {
    openModal() {
      this.modalOpen = true;
    },
    closeModal() {
      this.modalOpen = false;
    },
  },
};
</script>

<style>
.content__tabela {
  background: #fff;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.1);
  border-radius: 4px;
  justify-content: left;
  padding: 1.5em 0.5em;
}
</style>
