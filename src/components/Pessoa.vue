<template>
    <div>
        <h2>Essa é a descrição da pessoa: {{ name }}</h2>
        <Info />
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
            name: 'Thiago'
        }
    }
}
</script>