<template>
  <Header/>
  <primeiro-componente/>
  <life-cycle/>
  <pessoa/>
  <Form/>
  
</template>
<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import Form from './components/Form.vue';
import Header from './components/Header.vue';
export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Form,
    Header,
  }
}
</script>

<style>
body {
  background-color: darkcyan;
  color: aliceblue;
}
a {
  color: brown;
}

</style>