<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Novice></Novice>
        <Borrow></Borrow>
        <Money></Money>
        <Product></Product>
        <Life></Life>
        <Feeter></Feeter>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header"; //header组件和默认的HTML的header标签一致，所以要换名。
import Feeter from "../public/footer"; //y
import Navbar from "../public/navbar";
import Slider from "./hslider";
import Novice from "./novice";
import Borrow from "./borrow";
import Money from "./money";
import Product from "./product";
import Life from "./life";

export default {
  components: {
    Heador,
    Slider,
    Novice,
    Borrow,
    Money,
    Product,
    Life,
    Feeter,
    Navbar,
  }
};
</script>


