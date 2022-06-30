<template>
  <div id="main">
    <PrimeiroComponente />
    <LifeCycle />
  </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente'
import LifeCycle from './components/LifeCycle'


export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
  },
  data(){
    return{
      name: 'nada'
    }
  }
}
</script>

<style scoped>
*{
  padding: 0;
  margin: 0;
}

</style>