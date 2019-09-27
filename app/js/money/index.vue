<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Ada></Ada>
        <Money></Money>
        <Adb></Adb>
        <Finance></Finance>
        <Adc ></Adc>
        <Feeter cname="mfooter"></Feeter>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header"; //header组件和默认的HTML的header标签一致，所以要换名。
import Feeter from "../public/footer"; //y
import Navbar from "../public/navbar";
import Slider from "./mslider";
import Ada from "./ada";
import Money from "./money";
import Adb from "./adb";
import Finance from "./finance";
import Adc from "./adc";

export default {
  components: {
    Heador,
    Slider,
    Feeter,
    Navbar,
    Ada,
    Money,
    Adb,
    Finance,
    Adc,
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


