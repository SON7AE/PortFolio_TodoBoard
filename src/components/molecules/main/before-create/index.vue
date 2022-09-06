<template>
    <div class="before-create">
        <div class="before-create__text-box">
            <span class="before-create__text-box__label">How to start : </span>
            <div class="before-create__text-box__step">
                <span>1. Create a page</span>
                <span>2. Add boards to page</span>
            </div>
            <CreatePageButton>
                <template #label>Add New Page</template>
            </CreatePageButton>
        </div>
    </div>
</template>

<script>
import CreatePageButton from '~/components/atoms/CreatePageButton.vue';

export default {
    components: { CreatePageButton },
};
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
            margin-bottom: 30px;
        }
    }
}
</style>
