<template>
  <div class="logo">
    <img :src="imagem" :alt="descricao" />
  </div>
</template>

<script>
export default {
  name: "Logo",
  props: {
    imagem: {
      type: String,
      required: true,
    },
    descricao: {
      type: String,
      default: "",
    },
  },
};
</script>

<style scoped>
.logo {
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}

img {
  width: 15em;
  height: auto;
  display: block;
}
</style>
