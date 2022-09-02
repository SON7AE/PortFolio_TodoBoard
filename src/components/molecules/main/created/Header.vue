<template>
    <header class="header">
        <span class="header__title">Enter Title Here</span>
        <MainCreatedProgress />
        <div class="header__footer">
            <div class="header__footer__date">
                <Calendar>
                    <template #label>From</template>
                </Calendar>
                <Calendar>
                    <template #label>To</template>
                </Calendar>
            </div>
            <CreateBoardButton class="header__footer__button">
                <template #label>Add New Board</template>
            </CreateBoardButton>
        </div>
    </header>
</template>

<script>
import Calendar from '~/components/atoms/Calendar.vue';
import CreateBoardButton from '~/components/atoms/CreateBoardButton.vue';
import MainCreatedProgress from '~/components/molecules/main/created/Progress.vue';

export default {
    components: { Calendar, CreateBoardButton, MainCreatedProgress },
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

    &__title {
        font-family: 'Roboto', sans-serif;
        font-weight: 700;
        font-size: 36px;
        color: $created--color--basic;
    }
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
            color: $font--color--basic;
        }
    }
}
</style>
