<template>
    <header class="header">
        <Input size="large" />
        <MainCreatedPageProgress />
        <div class="header__footer">
            <div class="header__footer__date">
                <Calendar size="mini" length="200px">
                    <template #label>From</template>
                </Calendar>
                <Calendar size="mini" length="200px">
                    <template #label>To</template>
                </Calendar>
            </div>
            <CreateBoardButton class="header__footer__button" @click="createBoard">
                <template #label>Add New Board</template>
            </CreateBoardButton>
        </div>
    </header>
</template>

<script>
import Input from '~/components/atoms/Input.vue';
import Calendar from '~/components/atoms/Calendar.vue';
import CreateBoardButton from '~/components/atoms/CreateBoardButton.vue';
import MainCreatedPageProgress from '~/components/molecules/main/created/page/Progress.vue';

export default {
    components: { Input, Calendar, CreateBoardButton, MainCreatedPageProgress },
    setup() {
        const createBoard = () => {
            console.log('버튼이 클릭되었습니다.');
        };

        return { createBoard };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.header {
    display: flex;
    flex-direction: column;

    width: calc(100% - 50px);

    padding: 80px 30px 30px 20px;
    gap: 16px;
    background-color: $color--white--000;

    &__footer {
        display: flex;
        align-items: center;
        justify-content: space-between;

        &__date {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        &__button {
            width: 188px;
            color: $color--white--000;
        }
    }
}
</style>
