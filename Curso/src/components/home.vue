<template>
<div id="logo"> 
<h1> Teste {{2 + 2 * 5}}</h1>
<h1>{{nome}}</h1>
<hr>
<h1>{{numero}}</h1>
<hr>
<h1>{{email}}</h1>

<hr>
</div>
</template>

<script>
export default{
    data(){
        return {
            nome: "Nayron",
            numero:"31",
            email:"nhollupi@gmail.com",
            idade:0
        }
    } 
}
</script>

<style scoped>

</style>
