<template>
    <picture>
    <img :src="avatar" :alt="descricao">
    </picture>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue'

export default {
  components: { Reutilizacao },
    nome: 'Picture',
    data(){
        return{
            avatar: "/img/avatar.png",
            descricao: "Thiago Silva Andrade"
        }
    }
}
</script>