<script>
export default {
    name: 'AppHeader',
    props: ['message'],
};
</script>

<template>
    <header class="container">
        <h1 class="text-center my-5">
            {{ message }}
        </h1>
    </header>
</template>

<style scoped lang="scss">
h1 {
    font-weight: 700;
}
</style>