<template>
  <div id="app">
    <HeaderBar
            absolute
            prominent
    ></HeaderBar>
  </div>
</template>

<script>
  import HeaderBar from "./components/HeaderBar";

  export default {
    name: "App",
    data() {
      return {}
    },
    components: {
      HeaderBar
    }
  }
</script>

<style lang="less">
  html, body, #app {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    padding: 0;
    margin: 0;
    align-items: center;
    width: 100vw;
    min-height: 100vh;
    background: red;
  }

</style>
