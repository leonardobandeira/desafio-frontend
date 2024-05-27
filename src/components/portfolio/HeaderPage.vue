<template>
  <div class="row content__titulo">
    <span class="titulo">BTC Carteiras</span>
    <button class="btn__add__carteira">Adicionar Carteira</button>
  </div>
</template>

<script>
export default {};
</script>

<style>
.content__titulo {
  display: flex;
  justify-content: space-between;
}

.titulo {
  color: #000;
  font-size: 1.5em;
  font-weight: 700;
}

.btn__add__carteira {
  color: #fff;
  font-weight: 400;
  font-size: 1em;
  background-color: #007bff;
  padding: 0.4em 1em;
  border: #007bff;
  border-radius: 4px;
}
</style>