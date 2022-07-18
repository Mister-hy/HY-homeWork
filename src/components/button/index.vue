<template>
  <button
    :disabled="disabled"
    class="hy-button"
    :class="[style, isRadius, isBorder, isSize]"
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
    radius: Boolean,
    // 边框
    border: Boolean,
    // 大小
    size: {
      type: String,
      default: "",
    },
  },
  computed: {
    // 主题
    style() {
      return this.type ? `hy-button-${this.type}` : "";
    },
    // 圆角
    isRadius() {
      return this.radius ? "is-radius" : "";
    },
    // 边框
    isBorder() {
      return this.border ? "is-border" : "";
    },
    // 大小
    isSize() {
      return this.size ? `hy-button-${this.size}` : "";
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
