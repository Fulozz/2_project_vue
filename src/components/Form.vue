<template>
    <form name="meu_form" action="" @submit="enviarFormulario($event)">

  <h1>Entre em contato</h1>
    <div>
        <div><label for="nome">Nome</label></div>
  <input type="text" v-model="name" placeholder="Nome" />
</div>
    <div>
        <div><label for="email">Email</label></div>
  <input type="email" v-model="email" id="emailid" placeholder="exemplo@mail.com" name="email" />
  
</div>
    <div>
        <div><label for="email">Text</label></div>
    <textarea placeholder="Deixe sua opnião"></textarea>
    <input type="submit" class="enviar" onclick="Enviar();" value="Enviar" />
</div>
</form>
</template>
<script>
export default {
    name: 'Form',
    components:{

    },data(){
        return{
            name: '',
            email: ''
        }
    },
    methods: {
        enviarFormulario(e) {
            const name = this.name;
            const email = this.email;

            e.preventDefault();
            console.log("Formulario Enviado");
            console.log("O nome é: " + name);
            console.log("O email é: " + email);


            // Ajax

            // Inserir no banco de dados
        }
    }
}
</script>