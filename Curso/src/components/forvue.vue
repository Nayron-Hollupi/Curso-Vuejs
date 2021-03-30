<template>
    <div class="aula" >
        <h1>{{title}}</h1>
          <h1 >ID: {{cadastro.id}}</h1>
          <h1 >Nome: {{cadastro.nome}}</h1>
       <h1 >Email: {{cadastro.email}}</h1>
         <h1 >Idade: {{cadastro.idade}}</h1>  
     </div>
</template>

<script>
export default{
    data(){
        return {
         
        }
    },
     props: {
        cadastro: Object

    }


}

</script>

<style scoped>
.aula{
color:darkblue;
    background-color:rgb(233, 230, 230);
    padding: 2%;
    margin-top: 2%;
}

</style>