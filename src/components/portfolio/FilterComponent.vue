<template>
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
</template>

<script>
import FormInput from "./../form/FormInput";

export default {
  name: "FilterComponent",
  components: {
   FormInput,
  },
};
</script>

<style>
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
</style>