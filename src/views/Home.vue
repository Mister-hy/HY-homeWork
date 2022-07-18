<template>
  <div class="home">
    <HyButton radius>默认按钮</HyButton>
    <HyButton type="primary" size="medium" border>成功按钮</HyButton>
    <HyButton type="danger" size="small" radius>危险按钮</HyButton>
    <HyButton type="warning" size="mini" border>警告按钮</HyButton>
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
