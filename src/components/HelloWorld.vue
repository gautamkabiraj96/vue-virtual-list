<template>
  <div>
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
        { id: 2, title: "Title 2" },
        { id: 3, title: "Title 3" },
        { id: 4, title: "Title 4" },
        { id: 5, title: "Title 5" },
        { id: 6, title: "Title 6" },
        { id: 7, title: "Title 7" },
        { id: 8, title: "Title 8" },
        { id: 9, title: "Title 9" },
        { id: 10, title: "Title 10" },
        { id: 11, title: "Title 11" },
        { id: 12, title: "Title 12" },
        { id: 13, title: "Title 13" },
        { id: 14, title: "Title 14" },
        { id: 15, title: "Title 15" },
        { id: 16, title: "Title 16" },
        { id: 17, title: "Title 16" },
        { id: 18, title: "Title 16" },
        { id: 19, title: "Title 16" },
        { id: 20, title: "Title 16" },
        { id: 21, title: "Title 16" },
        { id: 22, title: "Title 16" },
        { id: 23, title: "Title 16" },
        { id: 24, title: "Title 16" },
        { id: 25, title: "Title 16" },
        { id: 26, title: "Title 16" },
        { id: 27, title: "Title 16" },
        { id: 28, title: "Title 16" },
        { id: 29, title: "Title 16" },
        { id: 30, title: "Title 16" },
        { id: 31, title: "Title 16" },
        { id: 32, title: "Title 16" },
      ],
    };
  },
  components: { "virtual-list": VirtualList },
};
</script>