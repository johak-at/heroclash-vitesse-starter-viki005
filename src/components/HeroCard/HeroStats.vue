<script setup>

const props = defineProps(['name', 'stats', 'alignment'])

</script>
<template>
    <div :class="alignment">
    <h1>{{ name }}</h1>
    <StatField v-for ="(value,key) in stats" :key="key" :skill="key" :value="value" />
    </div>
</template>

<style scoped>
.bad{
    background-image:linear-gradient(135deg, red, orange);
}

.good{
    background-image:linear-gradient(135deg, lightgreen, green);
}
.neutral{
    background-image: yellow;
}