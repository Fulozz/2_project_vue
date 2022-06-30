<template>
    <div class="primeiroComponente">
    <h1>Olá vue!! </h1>
    <p>Meu nome é {{ nome}} e sou um {{ profissao }} </p>
    </div>
</template>

<script>
export default {
    name: 'PrimeiroComponente',
    data(){
        return{
            nome: "Thiago",
            profissao: "Programador Junior"
        }
    }
}
</script>

<style scoped>
    .primeiroComponente{
        text-align: center;
    }
</style>