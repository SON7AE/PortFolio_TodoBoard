<template>
    <div class="main-section">
        <MainCreatedIndex v-if="page" />
        <MainBeforeCreateIndex v-else />
    </div>
</template>

<script>
import MainBeforeCreateIndex from '~/components/molecules/main/before-create/index.vue';
import MainCreatedIndex from '~/components/molecules/main/created/index.vue';

export default {
    components: { MainBeforeCreateIndex, MainCreatedIndex },
    props: {
        page: {
            type: Boolean,
            required: true,
            default: false,
        },
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.main-section {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 860px;
    height: 100vh;
    border-right: 1px solid $color--white--600;
}
</style>
