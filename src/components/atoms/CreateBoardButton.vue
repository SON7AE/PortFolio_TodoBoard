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

    background-color: $color--orange--000;
    border: 1px solid $color--orange--000;
    border-radius: 4px;
    color: $color--orange--000;
    font-family: 'Roboto', sans-serif;
    font-size: 14px;
    cursor: pointer;

    &:hover {
        background-color: $color--orange--100;
    }
    &__active {
        background-color: $color--orange--200;
        color: $color--orange--200;
    }
}
</style>
