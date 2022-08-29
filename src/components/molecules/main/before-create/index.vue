<template>
    <div class="before-create">
        <div class="before-create__text-box">
            <span class="before-create__text-box__label">How to start : </span>
            <div class="before-create__text-box__step">
                <span>1. Create a page</span>
                <span>2. Add boards to page</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.before-create {
    display: flex;
    align-items: center;
    justify-content: center;

    &__text-box {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

        gap: 16px;

        font-family: 'Roboto', sans-serif;
        line-height: 32px;

        &__label {
            font-weight: 700;
            font-size: 28px;
        }
        &__step {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;

            font-size: 18px;
        }
    }
}
</style>
