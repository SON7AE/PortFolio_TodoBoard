<template>
    <header class="header">
        <CheckBox />
        <span class="header__title">Enter Title Here</span>
    </header>
</template>

<script>
import CheckBox from '~/components/atoms/CheckBox.vue';

export default {
    components: {
        CheckBox,
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.header {
    display: flex;
    align-items: center;

    &__title {
        flex-grow: 1;

        border: 0;
        outline: 0;

        background: transparent;
        font-family: 'Roboto', sans-serif;
        font-size: 24px;
        font-weight: 600;
        color: $color--white--600;

        margin-left: 16px;
    }
}
</style>
