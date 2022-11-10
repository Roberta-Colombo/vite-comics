<template>
    <header>
        <div class="container">
            Sono header
        </div>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent'
        
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

    header {
        background-color: white;
        height: 110px;
        margin-top: 20px;
    }
</style>