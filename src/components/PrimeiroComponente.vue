<template>
    <div class="primeiroComponente">
    <h1>Olá vue!! </h1>
    <Reutilizacao />
    <p>Meu nome é {{ nome}} e sou um {{ profissao }} </p>
    <MultiplosEventos />
    <Reutilizacao />

    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos'
    import Reutilizacao from './Reutilizacao.vue'
export default {
    name: 'PrimeiroComponente',
    components:{
        MultiplosEventos,
        Reutilizacao
    },
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