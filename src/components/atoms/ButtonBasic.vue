<template>
    <button :data-theme="theme" class="button-basic">
        {{ label }}
    </button>
</template>

<script>
/**
 * @typedef {"defalut" | "red"} Theme
 */
export default {
    props: {
        label: {
            type: String,
            required: true,
        },
        theme: {
            /**@type {import("vue").PropType<Theme>} */
            type: String,
            required: false,
            /**@type {Theme} */
            default: 'default',
        },
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.button-basic {
    outline: 0;
    border: 0;
    background: transparent;
    font-family: 'Roboto', sans-serif;
    color: $color--black--200;
    cursor: pointer;

    &[data-theme='default'] {
        &:hover {
            color: $color--black--000;
        }
    }
    &[data-theme='red'] {
        &:hover {
            color: #f30000;
        }
    }
}
</style>
