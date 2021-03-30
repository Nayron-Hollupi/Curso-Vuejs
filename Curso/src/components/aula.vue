<template>
    <div id="aula">
        <h1>{{title}}</h1>
       <h1>Nome: {{cliente.nome}}</h1>
        <h1>Idade: {{cliente.idade}}</h1>
        <h1>Emai: {{cliente.email}}</h1>
        


        <p><input type="text" :value="usuario" ></p>
        <hr>
        
         <p><input type="text" v-model="senha" ></p>
        <hr>
        <h1>{{usuario}}</h1>
        <h1>{{idade}}</h1>
        <h1>{{email}}</h1>
        
        <p><button type="button" class="btn btn-primary">Enviar</button> </p>  
         </div>
</template>

<script>
export default{
    data(){
        return {
            title:"Login",
            
        }
    },
    props: {
        usuario: String,
        idade: Number,
        email: String,
        cliente: Object
    }


}
</script>

<style scoped>
#aula{
color:darkblue;
    background-color:rgb(233, 230, 230);
    padding: 2%;
    margin-top: 2%;
}
</style>
