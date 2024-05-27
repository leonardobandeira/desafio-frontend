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
  margin: 0 1em;
  font-size: 16px;
  width: 100%;
  min-width: 13em;
}
</style>