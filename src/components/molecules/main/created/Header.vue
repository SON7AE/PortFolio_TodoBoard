<template>
    <header class="header">
        <span class="header__title">Enter Title Here</span>
        <MainCreatedProgress />
        <div class="header__date">
            <Calendar>
                <template #label>From</template>
            </Calendar>
            <Calendar>
                <template #label>To</template>
            </Calendar>
        </div>
    </header>
</template>

<script>
import Calendar from '~/components/atoms/Calendar.vue';
import MainCreatedProgress from '~/components/molecules/main/created/Progress.vue';

export default {
    components: { MainCreatedProgress, Calendar },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.header {
    display: flex;
    flex-direction: column;

    width: 100%;
    padding: 80px 30px 30px 20px;
    gap: 16px;

    &__title {
        font-family: 'Roboto', sans-serif;
        font-weight: 700;
        font-size: 36px;
        color: $created--color--basic;
    }
    &__date {
        display: flex;
        align-items: center;
        gap: 20px;
    }
}
</style>
