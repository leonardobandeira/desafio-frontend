<template>
  <div class="content">
    <div class="row content__titulo">
      <span class="titulo">BTC Carteiras</span>
      <button class="btn__add__carteira">Adicionar Carteira</button>
    </div>

    <div class="row content__filter">
      <FormInput
        type="text"
        name="nome"
        id="nome"
        placeholder="Informe o nome do cliente"
      />
      <FormInput
        type="text"
        name="sobrenome"
        id="sobrenome"
        placeholder="Informe o sobrenome do cliente"
      />
      <FormInput
        type="text"
        name="email"
        id="email"
        placeholder="Informe o email do cliente"
      />
      <button class="btn__buscar">
        <i class="fa-solid fa-magnifying-glass icon__buscar"></i>Buscar
      </button>
    </div>

    <div class="row content__tabela">
      slkanalcasslkanalcasslkanalcasslkanalcassl
      kanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkan
      alcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcasslkanalcas
    </div>
  </div>
</template>

<script>
import FormInput from "./../components/FormInput";
export default {
  name: "Content",
  components: {
    FormInput,
  },
};
</script>

<style>
.content {
  grid-area: content;
  padding: 3em 10em 0 10em;
  background-color: #f8f8f8;
}

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

.content__filter {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  background: #fff;
  box-shadow: 0px 5px 5px rgba(0, 0, 0, 0.1);
  width: 100%;
  height: 4em;
  margin: 2em 0 2em 0;
  border-radius: 0.2em;
}

.btn__buscar {
  background: #fff;
  border: solid 0.12em #007bff;
  font-size: 1em;
  width: 7em;
  height: 2.4em;
  border-radius: 6px;
  color: #007bff;
}

.icon__buscar {
  padding-right: 1em;
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