<template>
    <div>
        <h1>Olá Estella</h1>
    <p>Meu nome é {{ nome }} e Trabalho como {{ profissao }} </p>
    </div>
</template>
<script>
export default {
    name: 'PrimeiroComponente',
    data() {
        return {
            nome: "Marcelo",
            profissao: "Analista"
        }
    }
}
</script>