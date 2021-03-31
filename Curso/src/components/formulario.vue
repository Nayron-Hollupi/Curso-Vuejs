<template>
   
<h1>Cadastro</h1>
<input type="text" placeholder="nome" v-model="nomeField"><br>
<input type="email" placeholder="email" v-model="emailField"><br>
<input type="number" placeholder="idade" v-model="idadeField"><br>
<button @click="cadastrarUsuario"  class="btn btn-primary">Cadastrar</button>
<hr>  
</template>

<script>
export default{
    data(){
        return {
          nomeField: "",
          emailField: "",
          idadeField: 0,

        }
    }, 
    props: {
        cliente: Object,
        showIdade: Boolean

    },
    methods:{
          cadastrarUsuario: function(){
this.cadastros.push({nome: this.nomeField, email: this.emailField, idade: this.idadeField, id: Date.now()})
          }
    }


}
/*
eventos @click 


*/
</script>

<style scoped>
.aula{
color:darkblue;
    background-color:rgb(233, 230, 230);
    padding: 2%;
    margin-top: 2%;
}
.cliente-P{
  color:rgba(212, 192, 7, 0.808);
    background-color:rgb(0, 0, 0);
    padding: 2%;
    margin-top: 2%;  
}
</style>