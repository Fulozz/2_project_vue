<template>
  <div id="main">
    <Header :esta_logado="false" />
    <PrimeiroComponente />
    <LifeCycle />
    <Pessoa />
    <Form />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import Header from './components/Header.vue'
import Form from './components/Form.vue'


export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Header,
    Form
  },
  data(){
    return{
      
    }
  }
}
</script>

<style>

  body{
  background-color: #333;
  color: #FFF;
}
  .teste > a{
  color: red;
}
.teste{
  background-color: #000;
}

</style>