<template>
    <div class="footer-bottom">
        <div class="container">
            Footer bottom
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterBottomComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.footer-bottom {
    background-color: $footergrey;
    height: 130px;
    color: $white;
}

</style>