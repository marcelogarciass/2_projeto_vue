<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }} </h2>
        <Info/>
        <form/>
    </div>
</template>
<script>
import Form from './Form.vue';
import Info from './Info.vue';

export default {
    name: "Pessoa",
    data() {
        return {
            nome: "Marcelo Garcia"
        };
    },
    components: { Info, Form }
}
</script>