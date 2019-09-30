<template lang="html">
    <div>
        <Heador></Heador>
        <h1>请登录</h1>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header"; //header组件和默认的HTML的header标签一致，所以要换名。
import Navbar from "../public/navbar";

export default {
  components: {
    Heador,
    Navbar,
  }
};
</script>

<style lang="scss">
  h1{
    margin: 195px;
    color: red;
  }
</style>
