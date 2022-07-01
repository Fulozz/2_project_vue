<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
export default {
    nome: 'Picture',
    data(){
        return{
            avatar: "/img/avatar.png",
            descricao: "Thiago Silva Andrade"
        }
    }
}
</script>