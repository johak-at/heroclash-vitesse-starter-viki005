<script setup>
const hero = ref({
  appearance: {
    eyeColor: 'Yellow',
    gender: 'Male',
    hairColor: 'No Hair',
    height: [
      '6\'8',
      '203 cm',
    ],
    race: 'Human',
    weight: [
      '980 lb',
      '441 kg',
    ],
  },
  biography: {
    aliases: [
      'Rick Jones',
    ],
    alignment: 'good',
    alterEgos: 'No alter egos found.',
    firstAppearance: 'Hulk Vol 2 #2 (April, 2008) (as A-Bomb)',
    fullName: 'Richard Milhouse Jones',
    placeOfBirth: 'Scarsdale, Arizona',
    publisher: 'Marvel Comics',
  },
  connections: {
    groupAffiliation: 'Hulk Family; Excelsior (sponsor), Avengers (honorary member); formerly partner of the Hulk, Captain America and Captain Marvel; Teen Brigade; ally of Rom',
    relatives: 'Marlo Chandler-Jones (wife); Polly (aunt); Mrs. Chandler (mother-in-law); Keith Chandler, Ray Chandler, three unidentified others (brothers-in-law); unidentified father (deceased); Jackie Shorr (alleged mother; unconfirmed)',
  },
  id: 1,
  images: {
    lg: 'images/lg/1-a-bomb.jpg',
    md: 'images/md/1-a-bomb.jpg',
    sm: 'images/sm/1-a-bomb.jpg',
    xs: 'images/xs/1-a-bomb.jpg',
  },
  name: 'A-Bomb',
  powerstats: {
    combat: 64,
    durability: 80,
    intelligence: 38,
    power: 24,
    speed: 17,
    strength: 100,
  },
  slug: '1-a-bomb',
  work: {
    base: '-',
    occupation: 'Musician, adventurer, author; formerly talk show host',
  },
})
</script>

<template>
    <HeroCard :hero="hero" />
</template>