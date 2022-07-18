<template>
  <div class="home">
    <HyButton>默认按钮</HyButton>
    <HyButton type="primary">成功按钮</HyButton>
    <HyButton type="danger">危险按钮</HyButton>
    <!-- <HyButton type="warning">警告按钮</HyButton> -->
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {
    HyButton: () => import("../components/button/index.vue"),
  },
};
</script>

<style lang="scss"></style>
