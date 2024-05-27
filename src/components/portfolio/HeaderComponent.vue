<template>
  <div class="row content__titulo">
    <slot name="left"></slot>
    <slot name="right"></slot>
  </div>
</template>


<script>
export default {
  name: "HeaderComponent",
};
</script>

<style>
.content__titulo {
  display: flex;
  justify-content: space-between;
}
</style>