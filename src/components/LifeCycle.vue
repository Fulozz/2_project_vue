<template>
    <h1> meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
    name: 'LifeCycle',
    data(){
        return{
            nome: 'Ainda não sei'
        }
    },
    created(){
        setTimeout(()=>{
            this.nome = 'None'
        }, 1000);
    },
    mounted() {
        setTimeout(()=>{
            this.nome = 'Thiago'
        }, 2000);
    },
    methods:{
        lifeCycle(){
            console.log("Executou")
        }
    }
}
</script>

<style scoped>

</style>