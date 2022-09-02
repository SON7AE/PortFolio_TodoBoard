<template>
    <div class="main-section">
        <!-- <MainBeforeCreateIndex /> -->
        <MainCreatedIndex />
    </div>
</template>

<script>
import MainBeforeCreateIndex from '~/components/molecules/main/before-create/index.vue';
import MainCreatedIndex from '~/components/molecules/main/created/index.vue';

export default { components: { MainBeforeCreateIndex, MainCreatedIndex } };
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.main-section {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 860px;
    border-right: 1px solid $layout--border--color;
}
</style>
