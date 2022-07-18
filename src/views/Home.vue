<template>
  <div class="home">
    <HyButton Hyradius>默认按钮</HyButton>
    <HyButton type="primary" Hyborder >成功按钮</HyButton>
    <HyButton type="danger" Hyradius>危险按钮</HyButton>
    <HyButton type="warning" Hyborder>警告按钮</HyButton>
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
