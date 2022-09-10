<template>
    <div class="created">
        <MainCreatedPageHeader />
        <MainCreatedBoardIndex v-if="board" />
        <MainCreatedPageMain v-else @createBoard="createBoard" />
    </div>
</template>

<script>
import MainCreatedPageHeader from '~/components/molecules/main/created/page/Header.vue';
import MainCreatedPageMain from '~/components/molecules/main/created/page/Main.vue';
import MainCreatedBoardIndex from '~/components/molecules/main/created/board/Index.vue';
import { ref } from '@vue/reactivity';

export default {
    components: { MainCreatedPageHeader, MainCreatedPageMain, MainCreatedBoardIndex },
    setup() {
        const board = ref(false);
        const createBoard = () => {
            board.value = true;
        };

        return { board, createBoard };
    },
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
