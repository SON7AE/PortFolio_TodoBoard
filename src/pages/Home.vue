<template>
    <div class="page">
        <SideSection @isCreateNewTask="isCreateNewTask" />
        <MainSection />
    </div>
</template>

<script>
import SideSection from '~/components/organisms/SideSection.vue';
import MainSection from '~/components/organisms/MainSection.vue';

export default {
    components: { SideSection, MainSection },
    setup() {
        const isCreateNewTask = () => {};
        return { isCreateNewTask };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.page {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;
    height: 100%;

    margin: auto;
}
</style>
