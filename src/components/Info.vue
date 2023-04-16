<template>
    <div>
        <h2>Aprendendo Vue js</h2>
        <h3>Vu js</h3>
        <p>No trabalho utilizo as seguintes tecnologias:</p>
        <p v-if="esta_trabalhando" > Estou trabalhando no momento</p>
        <p v-else>Preciso me recolocar no mercado</p>
        <ul>
            <li>VUEjs</li>
            <li>Java Script</li>
            <li>HTML</li>
        </ul>
        <p v-show="mostrar_email" >Mande uma mensagem para: {{ email }} </p>
        <p>Para acessar meu portifolio basta clicar no link <a v-bind:href=" meu_link " target="Blank" >clique aqui</a> </p>
        <Picture/>
    </div>
</template>
<script>
import Picture from './Picture.vue'
export default {
  components: { Picture },
    nome: 'Info',
    data() {
        return{
            esta_trabalhando: true,
            mostrar_email: false,
            email: 'marcelogarciass@hotmail.com',
            meu_link: 'https://google.com'
        }
    }
}
</script>