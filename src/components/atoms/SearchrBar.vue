<template>
    <div class="search-bar">
        <img src="~/assets/images/research.png" alt="" class="search-bar__icon" />
        <input type="text" placeholder="Search" class="search-bar__input" />
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.search-bar {
    display: flex;
    align-items: center;
    justify-content: space-between;

    height: 32px;

    padding: 8px 10px;
    gap: 8px;

    background-color: $color--white--200;
    border-radius: 4px;

    &__icon {
        width: 24px;
        height: 24px;
    }
    &__input {
        width: 234px;
        height: 100%;

        background: transparent;
        border: none;
    }
}
</style>
