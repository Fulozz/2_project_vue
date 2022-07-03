<template>
    <form name="meu_form">

  <h1>Entre em contato</h1>
    <div>
        <div><label for="nome">Nome</label></div>
  <input type="text" id="nomeid" placeholder="Tiago Vale" required="required" name="nome" />
</div>
    <div>
        <div><label for="email">Email</label></div>
  <input type="email" id="emailid" placeholder="exemplo@mail.com" name="email" />
  
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

    },
    methods: {
        enviarFormulario() {
            console.log("Formulario Enviado");
        }
    }
}
</script>