<script>
import { store } from './../store.js';

import SingleCharacter from './SingleCharacter.vue';

export default {
    name: "CharactersList",
    components: {
        SingleCharacter,
    },
    data() {
        return {
            store,
        }
    }
}


</script>


<template>
    <section class="container">

        <SingleCharacter v-for="character in store.charactersList" :details="character" />

    </section>
</template>


<style scoped lang="scss">
@use '../styles/partials/variables' as *;

h4 {
    text-transform: capitalize;

    &::after {
        content: '';
        display: block;
        width: 40px;
        height: 1px;
        margin: 1rem auto;
    }
}

img {
    box-shadow: 0 0 6px 3px rgba(#000, 0.15);
}
</style>