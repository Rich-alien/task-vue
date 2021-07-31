<template>
  <div>
    <MainComponent/>
    <SliderComponent/>
  </div>
</template>
<script>
// import HeaderComponent from "./components/header/header.component"
import MainComponent from "./pages/main/main.component"
import SliderComponent from "./pages/slider/slider.component"

export default {
  name: 'App',
  components: {
    MainComponent,
    SliderComponent
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}

body {
  width: auto;
  background-color: black;
  color: white;
  font-size: 18px;
  line-height: 22px;
}
</style>
