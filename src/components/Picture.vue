<template>
    <picture>
    <img :src="avatar" :alt="descricao">
    <MudarImagem @mudar-imagem="trocarImagem" />
    </picture>
</template>

<script>
import MudarImagem from './MudarImagem.vue'
import Reutilizacao from './Reutilizacao.vue'

export default {
  components: { Reutilizacao, MudarImagem },
    nome: 'Picture',
    data(){
        return{
            avatar: "/img/avatar.png",
            descricao: "Thiago Silva Andrade"
        }
    },
    methods:{
        trocarImagem(){
            this.avatar = "/img/avatar2.png"
 
        }
    }
}
</script>