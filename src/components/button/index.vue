<template>
  <button
    :disabled="disabled"
    class="hy-button hy-button-primary is-border is-radius"
    :class="[style, isRadius, isBorder]"
  >
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "index",
  props: {
    // 主题
    type: {
      type: String,
      default: "",
    },
    // 禁用
    disabled: Boolean,
    // 圆角
    Hyradius: Boolean,
    // 边框
    Hyborder: Boolean,
  },
  computed: {
    // 主题
    style() {
      return this.type ? `hy-button-${this.type}` : "";
    },
    // 圆角
    isRadius() {
      return this.Hyradius ? "is-radius" : "";
    },
    // 边框
    isBorder() {
      return this.Hyborder ? "is-border" : "";
    },
  },
  data() {
    return {};
  },
  mounted() {},
  methods: {},
  components: {},
};
</script>

<style lang="scss" scoped>
@import "./button.scss";
</style>
