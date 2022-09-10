<template>
    <header class="header">
        <CheckBox />
        <Input size="small" class="header__title" />
    </header>
</template>

<script>
import CheckBox from '~/components/atoms/CheckBox.vue';
import Input from '~/components/atoms/Input.vue';

export default {
    components: { Input, CheckBox },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.header {
    display: flex;
    align-items: center;

    &__title {
        flex-grow: 1;
        margin-left: 16px;
    }
}
</style>
