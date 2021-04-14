<template>
  <div class="list-style">{{ index }} - {{ source.title }}</div>
</template>
 
<script>
export default {
  name: "item-component",
  props: {
    index: {
      // index of current item
      type: Number,
    },
    source: {
      // here is: {uid: 'unique_1', text: 'abc'}
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
  padding: 10px 0px;
  margin: 6px 0;
}
</style>