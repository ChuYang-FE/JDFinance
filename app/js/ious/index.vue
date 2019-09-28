<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Welfare></Welfare>
        <Service></Service>
        <Feeter cname="mfooter"></Feeter>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header"; //header组件和默认的HTML的header标签一致，所以要换名。
import Feeter from "../public/footer"; //y
import Navbar from "../public/navbar";
import Slider from "./islider";
import Welfare from "./welfare";
import Service from "./service";

export default {
  components: {
    Heador,
    Slider,
    Feeter,
    Navbar,
    Welfare,
    Service,
  }
};
</script>

<style lang="scss">

</style>


