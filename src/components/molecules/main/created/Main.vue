<template>
    <div class="main">
        <div class="main__empty">
            <span class="main__empty__text-1">There is no board yet.</span>
            <span class="main__empty__text-2">Click the button and start flashing!</span>
            <div class="main__empty__button">+</div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.main {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;
    height: 100%;
    background: #f9f9f9;

    &__empty {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

        font-family: 'Roboto', sans-serif;
        color: #454545;
        margin: auto;

        &__text-1 {
            font-weight: 700;
            font-size: 24px;
        }
        &__text-2 {
            margin: 8px 0 20px 0;
        }
        &__button {
            display: flex;
            align-items: center;
            justify-content: center;

            width: 74px;
            height: 74px;
            border: 1px solid $button--border--color;
            border-radius: 50%;

            font-family: 'Roboto', sans-serif;
            font-size: 32px;
            color: $board--color--normal;

            margin-top: 20px;
            cursor: pointer;
        }
    }
}
</style>
