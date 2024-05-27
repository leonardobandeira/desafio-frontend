<template>
  <div class="row content__titulo">
    <Title tipo="primary" texto="BTC Carteiras"/>
    <Button tipo="adicionar" texto="Adicionar Carteira" acao="add" />
  </div>
</template>

<script>
import Title from "./../form/Title";
import Button from "./../form/Button";
export default {
  name: "HeaderPage",
  components: {
    Title,
    Button,
  },
};
</script>

<style>
.content__titulo {
  display: flex;
  justify-content: space-between;
}
</style>