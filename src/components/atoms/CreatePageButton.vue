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
@import '~/scss/main.scss';

.button {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 234px;
    height: 37px;

    background-color: $page--color--normal;
    border: 1px solid $border--color;
    border-radius: 4px;
    color: $font--color--hover;
    font-family: 'Roboto', sans-serif;
    font-size: 14px;
    cursor: pointer;

    &:hover {
        background-color: $page--color--hover;
    }
    &__active {
        background-color: $page--color--active;
        color: $font--color--active;
    }
}
</style>
