<template>
    <div>
        <h1>Login</h1>
        <p><input type="text" :value="usuario" ></p>
        <hr>
         <p><input type="text" v-model="senha" ></p>
        <hr>
        <h1>{{senha}}</h1>
        <p><input type="text" placeholder="Senha"></p>
        <p><button type="button" class="btn btn-primary">Enviar</button> </p>  
         </div>
</template>

<script>
export default{
    data(){
        return {
            usuario: " Usuario",
            senha: "senha",
            iddade: "31"
            
        }
    }
}
</script>

<style scoped>

</style>