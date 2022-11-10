<template>
    <main>
        <div class="container">
            <strong>-- Main content goes here --</strong>
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MainComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

main {
    background-color: black;
    height: 110px;
    color: white;
}

</style>