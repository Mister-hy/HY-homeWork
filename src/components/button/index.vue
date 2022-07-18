<template>
  <button disabled class="hy-button" :class="[style]">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "index",
  props: {
    type: {
      type: String,
      default: "",
    },
  },
  computed: {
    style() {
      return this.type ? `hy-button-${this.type}` : "";
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
.hy-button {
  border-width: 1px;
  border-style: solid;
  border-color: #dcdfe6;
  height: 40px;
  padding: 0 20px;
  background-color: #fff;
  border-radius: 4px;
  font-size: 14px;
  color: #606266;
  cursor: pointer;
}
// button组件封装 - 定义主题色
.hy-button-primary {
  background-color: #409eff;
  border-color: #409eff;
  color: #fff;
}
.hy-button-success {
  background-color: #00d100;
  border-color: #00d100;
  color: #fff;
}
.hy-button-danger {
  background-color: #e6a23c;
  border-color: #e6a23c;
  color: #fff;
}
.hy-button-warning {
  background-color: #f56c6c;
  border-color: #f56c6c;
  color: #fff;
}
// css 属性选择器[]
.hy-button[disabled] {
  cursor: not-allowed;
  // cursor: pointer;
  opacity: 0.5;
}
</style>
