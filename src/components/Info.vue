<template>
    <div>
        <p>No trabalho utilizo as seguintes tecnologias:</p>
        <p v-if="esta_trabalhando" > Estou trabalhando no momento</p>
        <p v-else>Preciso me recolocar no mercado</p>
        <ul>
            <li>VUEjs</li>
            <li>Java Script</li>
            <li>HTML</li>
        </ul>
        <p v-show="mostrar_email" >Mande uma mensagem para: {{ email }} </p>
    </div>
</template>
<script>
export default {
    nome: 'Info',
    data() {
        return{
            esta_trabalhando: true,
            mostrar_email: false,
            email: 'marcelogarciass@hotmail.com'
        }
    }
}
</script>