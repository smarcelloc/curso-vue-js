<template>
  <div id="app">
    <!-- INICIAL DOS COMPONENTES -->
    <!-- <HelloWorld /> -->
    <!-- <DataBinding /> -->
    <!-- <HTMLPuro /> -->
    <OnceRenderizacao />
  </div>
</template>

<!-- JS -->
<script>
// IMPORTAÇÃO
// import HelloWorld from "./Princípios/HelloWorld";
// import DataBinding from "./Princípios/DataBinding.vue";
// import HTMLPuro from "./Princípios/HTMLPuro";

import OnceRenderizacao from "./Princípios/OnceRenderização";

export default {
  name: "App",
  components: {
    //COMPONENTES
    // HelloWorld
    // DataBinding
    //HTMLPuro
    OnceRenderizacao
  }
};
</script>

<!-- CSS -->
<style>
body {
  margin: 0;
  padding: 0;
  background: #333;
  height: 100vh;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  display: flex;
  color: #fff;
}

#app {
  background-color: #111;
  padding: 1rem;
  margin: auto;
  border: 0.1rem dashed #adff2f;
  display: inline-block;
}
</style>