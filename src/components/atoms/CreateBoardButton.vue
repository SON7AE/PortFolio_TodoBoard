<template>
    <div class="button">
        <slot name="label"></slot>
    </div>
</template>

<script>
export default {
    setup() {},
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.button {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;
    height: 37px;

    background-color: $board--color--normal;
    border: 1px solid $button--border--color;
    border-radius: 4px;
    color: $font--color--normal;
    font-family: 'Roboto', sans-serif;
    font-size: 14px;
    cursor: pointer;

    &:hover {
        background-color: $board--color--hover;
    }
    &__active {
        background-color: $board--color--active;
        color: $font--color--active;
    }
}
</style>
