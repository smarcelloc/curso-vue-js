<template>
  <div>
    <h1 v-text="titulo"></h1>
    {{html}}
    <!-- SOLUÇÃO: DIRETIVA V-HTML para renderizar em tags de html -->
    <hr />
    <div v-html="html"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      titulo: "Curso de VUE JS + HTML PURO",
      html:
        "<span>Minha TAGs Não RENDERIZAM :( </span><strong>Protege contra XSS ATACK {{Não Funciona, OK interpolação}}"
    };
  }
};
</script>