<template>
    <div class="created">
        <MainCreatedHeader />
        <MainCreatedMain />
    </div>
</template>

<script>
import MainCreatedHeader from '~/components/molecules/main/created/Header.vue';
import MainCreatedMain from '~/components/molecules/main/created/Main.vue';

export default {
    components: { MainCreatedHeader, MainCreatedMain },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.created {
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    width: 100%;
}
</style>
