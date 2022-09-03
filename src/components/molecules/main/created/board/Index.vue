<template>
    <div class="board">
        <MainCreatedBoardHeader />
        <MainCreatedBoardMain />
        <div class="board__markdown">
            <ButtonBasic label="Add Markdown" />
        </div>
    </div>
</template>

<script>
import MainCreatedBoardHeader from '~/components/molecules/main/created/board/Header.vue';
import MainCreatedBoardMain from '~/components/molecules/main/created/board/Main.vue';
import ButtonBasic from '~/components/atoms/ButtonBasic.vue';

export default {
    components: { MainCreatedBoardHeader, MainCreatedBoardMain, ButtonBasic },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.board {
    display: flex;
    flex-direction: column;

    width: calc(100% - 108px);

    padding: 24px;
    gap: 30px;

    background: $color--white--000;
    border: 1px solid #ededed;
    box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);
    border-radius: 4px;

    margin: 30px 30px 0 30px;

    &__markdown {
        display: flex;
        align-items: center;
        justify-content: center;

        width: 100%;

        padding-top: 24px;
        border-top: 1px solid #ededed;
    }
}
</style>
