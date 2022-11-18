
<script setup>
const props = defineProps(['hero'])
const showBiography = ref(false)

</script>

<template>
    <HeroModal v-if="showBiography" @hideBiography ="showBiography = false" />
    <div grid class="heroCard">
    <HeroImage :imageUrl="hero.images.md"
    @showBiography="showBiography = true"/>
    <HeroStats :name="hero.name" 
    :stats="hero.powerstats" 
    :alignment="hero.biography.alignment"/>
    </div>
</template>

<style scoped>
.heroCard {
    grid-template-columns: 1fr 1.2fr;
}
</style>