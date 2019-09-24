<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
    </div>
</template>

<script>
import Heador from "../public/header"  //header组件和默认的HTML的header标签一致，所以要换名。
import Slider from "./hslider"
export default {
  components: {
    Heador,
    Slider,
  }
}
</script>


