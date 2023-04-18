<template>
    <div>
        <h2>Aprendendo Vue js</h2>
        <h3>Vu js</h3>
        <p>No trabalho utilizo as seguintes tecnologias:</p>
        <p v-if="esta_trabalhando"> Estou trabalhando no momento</p>
        <p v-else>Preciso me recolocar no mercado</p>
        <ul>
            <li v-for="(technology, index) in backend" v-bind:key="index"> {{ technology }} </li>
        </ul>
        <p>Utilizo as seguintes tecnologias para Frontend</p>
        <ul>
            <li v-for="technology in frontend" :key="technology.id" > {{ technology.language }} </li>
        </ul>
        <div>
            <button @click="showEmail"> {{ textoBotao }} </button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }} </p>
        <p>Para acessar meu portifolio basta clicar no link <a v-bind:href="meu_link" target="Blank">clique aqui</a> </p>
        <Picture />
    </div>
</template>

<script>
import Picture from './Picture.vue'
export default {
    components: { Picture },
    nome: 'Info',
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: false,
            email: 'marcelogarciass@hotmail.com',
            meu_link: 'https://google.com',
            textoBotao: 'Mostrar e-mail',
            backend: ['Java Script', 'Vue js', 'Pyton'],
            frontend: [
                { id: 1, language: 'HTML' },
                { id: 2, language: 'CSS' },
                { id: 3, language: 'VUe' },
            ]
        }
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if (!this.mostrar_email) {
                this.textoBotao = 'Mostrar e-mail'
            } else {
                this.textoBotao = 'Esconder e-mail'
            }
        }
    }

}
</script>