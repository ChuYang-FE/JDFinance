<template>
  <section :class="[panelClass, cname]">
    <h4>-{{ title }}-</h4>
    <slot></slot>
  </section>
</template>

<script>
export default {
  //接收自定义样式cname和标题title
  props: {
    cname: {
      type: String,
      default: "",
    },
    title: {
      type: String,
      default: "",
    },
  },
  //默认样式panelClass为默认的panel
  data() {
    return {
      panelClass: "panel",
    }
  },
}
</script>

<style lang="scss">
@import "../../css/element.scss";
.panel {
  @include panel;
}
</style>