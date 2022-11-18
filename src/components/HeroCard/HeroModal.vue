[10:44] Saller Josef
<template>
 <div class="modal" @click="emits('hideBiography')">
<ul>
<li v-for="(value, key) in biography" :key="key">
 <p>{{ key }}: {{ value }}</p>
</li><li v-for="(value, key) in appearance" :key="key">
 <p>{{ key }}: {{ value }}</p>
</li><li v-for="(value, key) in work" :key="key">
 <p>{{ key }}: {{ value }}</p>
 </li><li v-for="(value, key) in connections" :key="key">
<p>{{ key }}: {{ value }}</p>
</li>
 </ul>
</div>
</template>

[10:44] Saller Josef
<script setup>
const props = defineProps(['name', 'appearance', 'biography', 'connections', 'work'])
const emits = defineEmits(['hideBiography'])
</script>



<style scoped>
.modal
{
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1;
    width: 100vw;
    height: 100vh;
    background-color: rgba(255,0,255,0.4);
}
</style>