<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Daily></Daily>
        <In></In>
        <More></More>
        <Feeter cname="mfooter"></Feeter>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header"; //header组件和默认的HTML的header标签一致，所以要换名。
import Feeter from "../public/footer"; //y
import Navbar from "../public/navbar";
import Slider from "./rslider";
import Daily from "./daily";
import In from "./in";
import More from "./more";

export default {
  components: {
    Heador,
    Slider,
    Feeter,
    Navbar,
    Daily,
    In,
    More,
  }
};
</script>

<style lang="scss">
  .mfooter{
    margin-top: 0 !important;
    ul{
      li:first-child{
        display: none;
      }
    }
  }
</style>


