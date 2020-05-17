<template>
  <div id="hello">
    <h1>{{ titulo }}</h1>
    <h2>{{ subtitulo }}</h2>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      titulo: "Hello World",
      subtitulo: "Vue JS, Agora!"
    };
  }
};
</script>
