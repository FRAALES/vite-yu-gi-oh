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

        <div class="row">
            <div v-for="character in store.charactersList" :key="character.id" class="col-6 col-md-4 col-lg-3 mb5">
                <SingleCharacter :details="character" />
            </div>
        </div>


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