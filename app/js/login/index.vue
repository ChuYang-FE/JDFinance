<template lang="html">
    <div>
        <Heador></Heador>
        <Download></Download>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header"; //header组件和默认的HTML的header标签一致，所以要换名。
import Navbar from "../public/navbar";
import Download from "../special/download";

export default {
  components: {
    Heador,
    Navbar,
    Download,
  }
};
</script>

<style lang="scss">
</style>
