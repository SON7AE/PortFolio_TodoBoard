<template>
    <div class="main">
        <div class="main__date">
            <Calendar size="small" length="165px" style="outline: none">
                <template #label>From</template>
            </Calendar>
            <Calendar size="small" length="165px">
                <template #label>To</template>
            </Calendar>
        </div>
        <div class="main__button">
            <ButtonBasic label="Duplicate" />
            <ButtonBasic label="Delete" theme="red" />
        </div>
    </div>
</template>

<script>
import Calendar from '~/components/atoms/Calendar.vue';
import ButtonBasic from '~/components/atoms/ButtonBasic.vue';

export default { components: { Calendar, ButtonBasic } };
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.main {
    display: flex;
    align-items: center;
    justify-content: space-between;

    &__date {
        display: flex;
        align-items: center;
        gap: 8px;
    }
}
</style>
