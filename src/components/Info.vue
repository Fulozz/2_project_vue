<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>   
        <p>Utilizo as seguintes tecnologias</p>
        <ul>
            <li>JavaScript</li>
            <li>Python</li>
            <li>PHP</li>
        </ul>
        <div>
            <button @click="showEmail">{{textoBotao}}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>
import Picture from './Picture.vue'

export default {
    name:'Info',
    components: {
        Picture
    },
    data(){
        return{
            esta_trabalhando: false,
            mostrar_email: false,
            email: 'thiago.sandrade0720@gmail.com',
            meu_link: 'https://fulozz.github.io/portfolio/',
            textoBotao: 'Mostrar e-mail'
        }
    },
    methods: {
        showEmail(){
            this.mostrar_email = !this.mostrar_email
            //! é para contrario ou seja se clicar uma vez ele mostra (true) e se clicar de novo acontece ao contrario ou seja (false) 
            if(!this.mostrar_email){
                this.textoBotao = 'Mostrar e-mail'
            } else{
                this.textoBotao = 'Esconder e-mail'
            }
        }
    }
}
</script>