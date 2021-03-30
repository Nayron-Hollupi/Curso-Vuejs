<template>
    <div :class="{'aula': !isP, 'cliente-P': isP}" >
        <h1>{{title}}</h1>
       <h1 >Nome: {{cliente.nome}}</h1>
        <h1 >Idade: {{cliente.idade}}</h1>  
       <h1 >Email: {{cliente.email}}</h1>
      <button @click="mudarCor($event)" type="button" class="btn btn-primary" >Mudar cor!</button>  
     </div>
</template>

<script>
export default{
    data(){
        return {
            title:"Eventos",
           isP: true 
        }
    },
    props: {
        cliente: Object,
        showIdade: Boolean

    },
    methods:{
        mudarCor: function($event){
            console.log($event);
           this.isP = !this.isP;
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