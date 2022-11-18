<script setup> 
    const props = defineProps(['imageUrl'])
    const emits = defineEmits('showBiography')
</script>

<template>
    <img :src="`https://raw.githubusercontent.com/akabab/superhero-api/master/.backup/${imageUrl}`" alt="Hero Image" @click="emits('showBiography')">
</template>