<template>
  <MainComponent/>
</template>
<script>
// import HeaderComponent from "./components/header/header.component"
import MainComponent from "./pages/main/main.component"

export default {
  name: 'App',
  components: {
    MainComponent
  }
}
</script>

<style lang="scss">
* {
  color: white;
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
