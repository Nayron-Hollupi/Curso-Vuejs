<template>

<h1>Cadastro</h1>
<small id="nomeErro" v-show="deuErro">O nome é invalido</small><br>
<input type="text" placeholder="nome" v-model="nomeField"><br>
<input type="email" placeholder="email" v-model="emailField"><br>
<input type="number" placeholder="idade" v-model="idadeField"><br>
<button @click="cadastrarUsuario"  class="btn btn-primary">Cadastrar</button>
<hr>  
<br>
     <div :class="{'aula': !isP, 'cliente-P': isP}" >
        <div v-for="cadastro in cadastros" :key="cadastro.id">
            <br>
      <h2>Nome:{{cadastro.nome}}</h2> 
        <h1 >Idade: {{cadastro.idade}}</h1>  
       <h1 >Email: {{cadastro.email}}</h1>
      <button @click="mudarCor($event)" type="button" class="btn btn-primary" >Mudar cor!</button>  

        </div>
     </div>
</template>

<script>
export default{
    data(){
        return {
             nomeField: "",
          emailField: "",
          idadeField: 0,
               title:"Eventos",
           isP: true,
            cadastros: [
    {
      id: 1,
  nome: "Nayron",
  email:"teste@teste",
  idade: 31
  },
 {
   id: 2,
  nome: "Daiane",
      email:"Daia@teste",
      idade: 27
  },
  {
    id: 3,
  nome: "Cleide",
      email:"Veia@teste",
      idade: 100
  },
  ], 
        }
    },
    methods:{
        mudarCor: function($event){
            console.log($event);
           this.isP = !this.isP;
        },
                cadastrarUsuario: function(){
                    if(this.nomeField == "" || this.nomeField == " " || this.nomeField < 3){
                       this.deuErro = true;
                    }else{
this.cadastros.push({nome: this.nomeField, email: this.emailField, idade: this.idadeField, id: Date.now()})
         this.nomeField = "";
         this.idadeField = 0;
         this.emailField = "";
         this.deuErro = false;
                    }
         }
    },
     



}

</script>

<style scoped>
.aula{
color:rgb(240, 226, 27);
    background-color:rgb(6, 20, 212);
    padding: 2%;
    margin-top: 2%;
}
.cliente-P{
  color:rgba(165, 10, 10, 0.808);
    background-color:rgb(2, 184, 33);
    padding: 2%;
    margin-top: 2%;  
}
#nomeErro{
    color:red;
}
</style>