<script>
import axios from 'axios';
import AppHeader from './components/AppHeader.vue'
import CharactersList from './components/CharactersList.vue'


export default {
  components: {
    AppHeader,
    CharactersList,
  }
}
</script>

<template>
  <AppHeader message="Yugi-oh Api" />
  <CharactersList />
</template>

<style lang="scss">
@use './styles/general' as *;
@use './styles/partials/variables' as *;
</style>
