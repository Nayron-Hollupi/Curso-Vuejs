<template>
    <div id="aula" >
        <h1>{{title}}</h1>
       <h1 >Nome: {{cliente.nome}}</h1>
        <h1 v-if="showIdade">Idade: {{cliente.idade}}</h1>
       <h1 v-else>Não colocou idade</h1>
     <h1 v-show="showIdade == true">Idade: {{cliente.idade}}</h1>
     
       <h1 >Email: {{cliente.email}}</h1>
  <p><button type="button" class="btn btn-primary">Enviar</button> </p>  
       
      
     </div>
</template>

<script>
export default{
    data(){
        return {
            title:"Aula1",
            
        }
    },
    props: {
        cliente: Object,
        showIdade: Boolean

    }


}
/*
----Deretivar do vue 
v-text
Em vez de usar a interpolação, você pode usar a diretiva v-text.

v-once
Você sabe como o {{name}} se liga à propriedade name nos dados do componente.

v-html
Quando você usa a interpolação para imprimir uma propriedade de dados, o HTML é escapado.

v-bind
A interpolação só funciona no conteúdo da tag. Você não pode usá-lo em atributos.

v-model

v-show exibe a mais o resultado fica escondido não deleta o elemento  
v-if ,v-else, v-else-if  Serve para esconder ou mostrar algo baseando em uma condição 
v-for


*/
</script>

<style scoped>
#aula{
color:darkblue;
    background-color:rgb(233, 230, 230);
    padding: 2%;
    margin-top: 2%;
}
</style>
