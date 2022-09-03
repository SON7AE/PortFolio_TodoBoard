<template>
    <div class="calendar" :style="{ width: length }">
        <span class="calendar__label">
            <slot name="label"></slot>
        </span>
        <ElDatePicker v-model="value1" type="date" placeholder="Pick a day" :size="size" />
    </div>
</template>

<script>
import { ref } from '@vue/reactivity';

export default {
    props: {
        size: {
            type: String,
            required: true,
            default: 'large',
        },
        length: {
            type: String,
            required: true,
            default: '200px',
        },
    },
    setup() {
        const value1 = ref('');

        return { value1 };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.calendar {
    display: flex;
    align-items: center;

    gap: 10px;

    &__label {
        font-family: 'Roboto', sans-serif;
        color: $color--black--200;
    }
}
</style>
