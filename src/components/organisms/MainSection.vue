<template>
    <div class="main-section">
        <BeforeCreateIndex />
    </div>
</template>

<script>
import BeforeCreateIndex from '~/components/molecules/main/before-create/index.vue';

export default { components: { BeforeCreateIndex } };
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.main-section {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 860px;
}
</style>
