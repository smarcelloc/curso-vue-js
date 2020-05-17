<template>
  <div>
    <p>Curso: {{nome}}</p>
    <!-- errado "{{}}": não permite
    <a href="{{documentação}}"></a>-->
    <!-- Solução: v-bind:href="{{***}}" -->
    <!-- v-bind:attr="variavel" é diretiva 
        sem interpolação "{{" "}}"
        DIRETIVA: É PROPRIEDADE DO VUE
    -->
    <a v-bind:href="documentação">Documentação</a>
    <hr />
    <!-- Permite pelo JS propriedade element.TEXT = texto -->
    <span v-text="texto"></span>
  </div>
</template>

<script>
export default {
  //name: "DataBinding"
  data() {
    return {
      nome: "Vue JS",
      documentação: "https://vuejs.org/",
      texto:
        "Adipisci corrupti ab deserunt eligendi eos qui corporis. Debitis rerum hic ipsam ut. Ullam dolores molestiae et debitis repudiandae molestiae sunt sint soluta. Laborum sed dolorum omnis dignissimos qui dolorum."
    };
  }
};
</script>