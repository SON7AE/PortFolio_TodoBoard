<template>
    <input :data-size="size" type="text" placeholder="Enter Title Here" />
</template>

<script>
/**
 * @typedef {"small", "large"} Size
 */
export default {
    props: {
        size: {
            /**@type {import("vue").PropType<Size>} */
            type: String,
            required: true,
            /**@type {Size} */
            default: 'small',
        },
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

input[type='text'] {
    outline: 0;
    border: none;
    background-color: transparent;

    font-family: 'Roboto', sans-serif;
}
input[data-size='small'] {
    font-size: 24px;
    font-weight: 600;

    &::placeholder {
        font-family: 'Roboto', sans-serif;
        font-weight: 700;
        font-size: 24px;
        color: $color--white--600;
    }
}
input[data-size='large'] {
    font-size: 36px;
    font-weight: 700;

    &::placeholder {
        font-family: 'Roboto', sans-serif;
        font-weight: 700;
        font-size: 36px;
        color: $color--white--600;
    }
}
</style>
