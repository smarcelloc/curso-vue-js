<template>
  <div>
    <!-- 
    Resultado : 
        Nome 1: Júlia,
        Nome 2: Júlia
        Porque o método setNome(nome) alterar a variavel (atributo) "nome"
    -->
    <!-- <h1>SEM V-ONCE</h1>
    <ul>
      <li>Nome 1: {{nome}}</li>
      <li>Nome 2: {{setNome('Júlia')}}</li>
    </ul>-->



    
    <!-- 
        TEMOS UMA SOLUÇÃO:
        - DIRETIVA V-ONCE
           Somente única renderização,
           Depois disso, mantém estático
        
        - Resultado:
            Nome 1: Fernando
            Nome 2: Júlia

    -->
    <hr />
    <h1>COM V-ONCE</h1>
    <ul>
      <li v-once>Nome 1: {{nome}}</li>
      <li>Nome 2: {{setNome('Júlia')}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nome: "Fernando"
    };
  },
  methods: {
    setNome: function(nome) {
      this.nome = nome;
      return this.nome;
    }
  }
};
</script>