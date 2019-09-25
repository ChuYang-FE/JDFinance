<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Novice></Novice>
        <Borrow></Borrow>
        <Money></Money>
    </div>
</template>

<script>
import Heador from "../public/header"  //header组件和默认的HTML的header标签一致，所以要换名。
import Slider from "./hslider"
import Novice from "./novice"
import Borrow from "./borrow"
import Money from "./money"
export default {
  components: {
    Heador,
    Slider,
    Novice,
    Borrow,
    Money,
  },
}
</script>


