<template>
  <div class="list-style">{{ index }} - {{ source.title }}</div>
</template>
 
<script>
export default {
  name: "item-component",
  props: {
    index: {
      type: Number,
    },
    source: {
      type: Object,
      default() {
        return {};
      },
    },
  },
};
</script>

<style scoped>
.list-style {
  border: 1px solid #eee;
  background: #eee;
  padding: 10px 8px;
  margin: 6px 0;
  text-align: left;
}
</style>