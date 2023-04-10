<template>
    <div>
        <h1>Meu nome é {{ nome }} </h1>
    </div>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
        nome: 'Ainda não sei'
        }
    },
    created() {
        setTimeout(() => {
            this.nome = 'Marcelo'
        }, 1000);
    },
    mountedgit() {
        setTimeout(() => {
            this.nome = 'Garcia'
        }, 2000);
    }
}
</script>