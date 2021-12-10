<template>
  <div class="container" ref="container"></div>
</template>

<script>
import LogicFlow from "@logicflow/core";
import "@logicflow/core/dist/style/index.css";

export default {
  mounted() {
    this.lf = new LogicFlow({
      container: this.$refs.container,
    });
    this.lf.render({
      nodes: [
        {
          id: "1",
          type: "rect",
          x: 100,
          y: 100,
        },
        {
          id: "2",
          type: "circle",
          x: 300,
          y: 200,
        },
      ],
      edges: [
        {
          sourceNodeId: "1",
          targetNodeId: "2",
          type: "polyline",
        },
      ],
    });
  },
};
</script>

<style scoped>
.container {
  width: 100%;
  height: 100%;
}
</style>