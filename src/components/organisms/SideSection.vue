<template>
    <div class="side-section">
        <AsideHeader />
        <AsideMain />
    </div>
</template>

<script>
import AsideHeader from '~/components/molecules/aside/Header.vue';
import AsideMain from '~/components/molecules/aside/Main.vue';

export default {
    components: { AsideHeader, AsideMain },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.side-section {
    display: flex;
    flex-direction: column;

    width: 282px;
    height: calc(100vh - 156px);

    padding: 78px 24px;
    gap: 26px;

    border-left: 1px solid $layout--border--color;
    border-right: 1px solid $layout--border--color;
}
</style>
