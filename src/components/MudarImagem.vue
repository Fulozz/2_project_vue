<template>
    <div>
        <button @click="$emit('mudarImagem')">Trocar imagem de perfl</button>
    </div>    
</template>
<script>
export default {
    name: 'MudarImagem',

    emits: ['mudarImagem']
}
</script>
<style scoped>

</style>