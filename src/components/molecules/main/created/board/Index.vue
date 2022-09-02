<template>
    <div class="board">
        <MainCreatedBoardHeader />
        <MainCreatedBoardMain />
    </div>
</template>

<script>
import MainCreatedBoardHeader from '~/components/molecules/main/created/board/Header.vue';
import MainCreatedBoardMain from '~/components/molecules/main/created/board/Main.vue';

export default {
    components: { MainCreatedBoardHeader, MainCreatedBoardMain },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.board {
    display: flex;
    flex-direction: column;

    width: calc(100% - 108px);
    height: 187px;

    padding: 24px;
    gap: 30px;

    background: #ffffff;
    border: 1px solid #ededed;
    box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);
    border-radius: 4px;

    margin: 30px 30px 0 30px;
}
.select-box {
    display: flex;
    align-items: center;
}
</style>
