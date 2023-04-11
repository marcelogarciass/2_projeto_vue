<template>
        <h2>Meu Formulario</h2>
        <form action="">
            <div>
                <input-text/>
            </div>
            <div>
                <input-text/>
            </div>
            <div>
                <submit/>
            </div>
        </form>
    
</template>
<script>
import inputText from './form/inputText.vue'
import Submit from './form/Submit.vue'
export default {
  components: { inputText, Submit },
    name: 'Form'
}
</script>