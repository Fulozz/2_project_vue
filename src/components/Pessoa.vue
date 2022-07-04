<template>
    <div>
        <h2>Essa é a descrição da pessoa: {{ name }}</h2>
        <Info :email="email" :esta_trabalhando="false" />
    </div>
</template>
<script>
    import Info from './Info.vue'

export default {
    name: 'Pessoa',
    components:{
        Info
    },
    data(){
        return{
            name: 'Thiago',
            email: 'thiago.sandrade0720@gmail.com'
        }
    }
}
</script>