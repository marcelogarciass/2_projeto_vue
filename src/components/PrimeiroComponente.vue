<template>
    <Reutilizacao/>
    <div>
        <h1>Olá Marcelo</h1>
    <p>Meu nome é {{ nome }} e Trabalho como {{ profissao }} </p>
    </div>
    <Reutilizacao/>
</template>
<script>
import Reutilizacao from './Reutilizacao.vue';

export default {
    name: "PrimeiroComponente",
    data() {
        return {
            nome: "Marcelo",
            profissao: "Analista"
        };
    },
    components: { Reutilizacao }
}
</script>