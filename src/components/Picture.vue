<template>
    <div>
        <p><img :src="avatar" :alt="descricao"></p>
    </div>
</template>
<script>
    export default {
    name: 'Picture',
    data() {
        return {
            avatar: '/img/avatar.jpg',
            descricao: 'Marcelo Garcia'
        }
    }
}
</script>