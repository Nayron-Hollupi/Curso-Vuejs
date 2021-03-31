<template>

<Cadastro/>

</template>

<script>
//import home from './components/home';
//import login from './components/login';
import Cadastro from './components/Cadastro';
//import aula2 from './components/aula2';
//import eventos from './components/eventos';
//import formulario from './components/formulario';

export default{ data(){
    return{
      usuarioNayron: "Victor Hollupi",
      clienteN:{
        nome: "Hollupi",
      email:"Mer@tet@",
      idade:"55"
  },

}
},
  

  components:{
   // home,
  // login,
Cadastro,
  //aula2,
 // eventos,
 // formulario
 
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

  