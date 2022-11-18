<script setup>
    const props=defineProps(['skill', 'value'])
    const icon = computed (() => {

switch(props.skill){

    case 'intelligence':
        return 'i-game-icons-brain';
    case 'strength':
        return 'i-game-icons-biceps';
    case 'speed':
        return 'i-game-icons-running-ninja';
    case 'durability':
        return 'i-game-icons-crenulated-shield';
    case 'power':
        return 'i-game-icons-fist';
    case 'combat':
        return 'i-game-icons-crossed-swords';

}

})
</script>

<template>

    <div flex justify-between>
         <span> <div :class="icon" inline-block/> {{ skill[0].toUpperCase()+skill.substring(1,skill.length) }}</span>
         <span> {{ value }}</span>
    </div>
</template>