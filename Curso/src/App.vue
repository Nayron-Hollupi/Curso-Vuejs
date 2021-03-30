<template>
<eventos :cliente="clienteN" :showIdade="true"/>

<eventos :cliente="clienteN" :showIdade="false"/>
</template>

<script>
//import home from './components/home';
//import login from './components/login';
//import forvue from './components/forvue';
//import aula2 from './components/aula2';
import eventos from './components/eventos';

export default{ data(){
    return{
      usuarioNayron: "Victor Hollupi",
      clienteN:{
        nome: "Hollupi",
      email:"Mer@tet@",
      idade:"55"
  },
  cadastro: [
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
  ]
}
},
  

  components:{
   // home,
  // login,
//forvue,
  //aula2,
  eventos
 
  }
}

</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

  