<template>
    <div :class="{'aula': !isP, 'cliente-P': isP}" >
        <h1>{{title}}</h1>
       <h1 >Nome: {{cliente.nome}}</h1>
        <h1 >Idade: {{cliente.idade}}</h1>  
       <h1 >Email: {{cliente.email}}</h1>
       <hr>npm run   
     </div>
</template>

<script>
export default{
    data(){
        return {
            title:"Aula1",
           isP: true 
        }
    },
    props: {
        cliente: Object,
        showIdade: Boolean

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
.cliente-P{
  color:rgba(212, 192, 7, 0.808);
    background-color:rgb(0, 0, 0);
    padding: 2%;
    margin-top: 2%;  
}
</style>