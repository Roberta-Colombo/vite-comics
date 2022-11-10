<template>
    <section class="blue-bar">
        <div class="container">
            Sono la barra blu
        </div>
    </section>
</template>

<script>
    export default {
        name: 'BlueBarComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.blue-bar {
    background-color: $skyblue;
    height: 160px;
    color: $white;
}

</style>