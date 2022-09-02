<template>
    <button :class="{ delete: isDelete }" class="button-basic">
        {{ label }}
    </button>
</template>

<script>
import { computed } from '@vue/reactivity';
export default {
    props: {
        label: {
            type: String,
            required: true,
        },
    },
    setup(props) {
        const isDelete = computed(() => {
            if (props.label === 'Delete') true;
        });

        return {
            isDelete,
        };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.button-basic {
    outline: 0;
    border: 0;
    background: transparent;
    cursor: pointer;

    &__active {
        &:hover {
            color: red;
        }
    }

    &:hover {
        color: #00f38d;
    }
}
</style>
