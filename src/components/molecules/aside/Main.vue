<template>
    <div class="main">
        <span class="main__user-name">Park's</span>
        <div class="main__contents">
            <AsideContent />
        </div>
    </div>
</template>

<script>
import AsideContent from '~/components/molecules/aside/Content.vue';

export default {
    components: {
        AsideContent,
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.main {
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    width: 100%;

    &__user-name {
        font-family: 'Roboto', sans-serif;
        font-size: 16px;
        font-weight: 600;
        color: $color--white--700;
        margin-bottom: 8px;
    }
    &__contents {
        width: 100%;
    }
}
</style>
