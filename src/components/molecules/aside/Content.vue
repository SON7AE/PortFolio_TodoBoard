<template>
    <div class="content">
        <span class="content__dot"></span>
        <span class="content__title">Dev env setting</span>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.content {
    display: flex;
    align-items: center;

    padding: 10px 7px;
    cursor: pointer;

    &__dot {
        width: 6px;
        height: 6px;
        background-color: $color--green--000;
        border-radius: 50%;
        margin-right: 10px;
    }
    &__title {
        font-family: 'Roboto', sans-serif;
        font-size: 16px;
        font-weight: 600;
    }
    &:hover {
        background-color: $color--white--300;
    }
}
</style>
