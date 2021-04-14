<template>
  <div>
    <h2>Virtual list example</h2>
    <virtual-list
      style="height: 360px; overflow-y: auto"
      scrollable
      :data-key="'id'"
      :data-sources="items"
      :data-component="itemComponent"
    />
  </div>
</template>
 
<script>
import Item from "./ListItem";
import VirtualList from "vue-virtual-scroll-list";

export default {
  name: "root",
  data() {
    return {
      itemComponent: Item,
      items: [
        { id: 1, title: "Gautam" },
        { id: 2, title: "Night" },
        { id: 3, title: "Programmer" },
        { id: 4, title: "Gautam" },
        { id: 5, title: "Night" },
        { id: 6, title: "Programmer" },
        { id: 7, title: "Gautam" },
        { id: 8, title: "Night" },
        { id: 9, title: "Programmer" },
        { id: 10, title: "Gautam" },
        { id: 11, title: "Night" },
        { id: 12, title: "Programmer" },
        { id: 13, title: "Gautam" },
        { id: 14, title: "Night" },
        { id: 15, title: "Programmer" },
        { id: 16, title: "Gautam" },
        { id: 17, title: "Night" },
        { id: 18, title: "Programmer" },
        { id: 19, title: "Gautam" },
        { id: 20, title: "Night" },
        { id: 21, title: "Programmer" },
        { id: 22, title: "Gautam" },
        { id: 23, title: "Night" },
        { id: 24, title: "Programmer" },
        { id: 25, title: "Gautam" },
        { id: 26, title: "Night" },
        { id: 27, title: "Programmer" },
        { id: 28, title: "Gautam" },
        { id: 29, title: "Night" },
        { id: 30, title: "Programmer" },
        { id: 31, title: "Gautam" },
        { id: 32, title: "Night" },
        { id: 33, title: "Programmer" },
        { id: 34, title: "Gautam" },
        { id: 35, title: "Night" },
        { id: 36, title: "Programmer" },
        { id: 37, title: "Gautam" },
        { id: 38, title: "Night" },
        { id: 39, title: "Programmer" },
        { id: 40, title: "Gautam" },
        { id: 41, title: "Night" },
        { id: 42, title: "Programmer" },
        { id: 43, title: "Gautam" },
        { id: 44, title: "Night" },
        { id: 45, title: "Programmer" },
        { id: 46, title: "Gautam" },
        { id: 47, title: "Night" },
        { id: 48, title: "Programmer" },
        { id: 49, title: "Gautam" },
        { id: 50, title: "Night" },
        { id: 51, title: "Programmer" },
        { id: 52, title: "Gautam" },
        { id: 53, title: "Night" },
        { id: 54, title: "Programmer" },
        { id: 55, title: "Gautam" },
        { id: 56, title: "Night" },
        { id: 57, title: "Programmer" },
        { id: 58, title: "Gautam" },
        { id: 59, title: "Night" },
        { id: 60, title: "Programmer" },
      ],
    };
  },
  components: { "virtual-list": VirtualList },
};
</script>