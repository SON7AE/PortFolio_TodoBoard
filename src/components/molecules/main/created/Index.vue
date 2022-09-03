<template>
    <div class="created">
        <MainCreatedPageHeader />
        <!-- <MainCreatedPageMain /> -->
        <MainCreatedBoardIndex />
    </div>
</template>

<script>
import MainCreatedPageHeader from '~/components/molecules/main/created/page/Header.vue';
import MainCreatedPageMain from '~/components/molecules/main/created/page/Main.vue';
import MainCreatedBoardIndex from '~/components/molecules/main/created/board/Index.vue';

export default {
    components: { MainCreatedPageHeader, MainCreatedPageMain, MainCreatedBoardIndex },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.created {
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    width: 100%;
    height: 100%;

    background: $color--white--400;
}
</style>
