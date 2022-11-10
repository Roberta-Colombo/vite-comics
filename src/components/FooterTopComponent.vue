<template>
    <div class="footer-top">
        <div class="container">
            Footer top
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterTopComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.footer-top {
    background-image: url("../assets/img/footer-bg.jpg");
    height: 350px;
    color: $white;
}
</style>