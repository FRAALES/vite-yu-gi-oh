<script>
export default {
    name: "SingleCharacter",
}
</script>


<template>
    <!-- card character di esempio -->
    <div class="character text-center">
        <img src="info.image" alt="info.name" class="img-fluid mb-3">
        <h4>name</h4>
        <div class="font-weight-bold">archetype</div>
    </div>
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