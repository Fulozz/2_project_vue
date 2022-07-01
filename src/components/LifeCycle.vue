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
            this.lifeCycle()
    },
    mounted() {
        setTimeout(()=>{
            this.nome = 'Thiago'
        }, 2000);
            this.lifeCycle() 
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