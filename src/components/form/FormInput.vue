<template>
  <div class="">
    <input
      class="item__campo"
      :type="text"
      :name="nome"
      :id="id"
      :placeholder="placeholder"
    />
  </div>
</template>

<script>
export default {
  props: {
    type: {
      type: String,
      default: "text",
    },
    name: {
      type: String,
      required: true,
    },
    id: {
      type: String,
      required: true,
    },
    placeholder: {
      type: String,
      default: "",
    },
  },
};
</script>

<style>
.item__campo {
  border: 0.1em solid #007bff;
  padding: 8px;
  border-radius: 4px;
  font-size: 16px;
  width: 17em;
  max-width: 17em;
}
</style>