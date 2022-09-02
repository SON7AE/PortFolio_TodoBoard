<template>
    <div class="calendar">
        <span class="calendar__label">
            <slot name="label"></slot>
        </span>
        <ElDatePicker v-model="value1" type="date" placeholder="Pick a day" :size="size" />
    </div>
</template>

<script>
import { ref } from '@vue/reactivity';

export default {
    setup() {
        const value1 = ref('');
        const size = ref('large');

        return { value1, size };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.calendar {
    display: flex;
    align-items: center;

    width: 200px;
    gap: 10px;

    &__label {
        font-family: 'Roboto', sans-serif;
        color: #6d6d6d;
    }
}
</style>
