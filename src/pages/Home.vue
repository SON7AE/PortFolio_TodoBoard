<template>
    <div class="page">
        <SideSection @createPage="createPage" />
        <MainSection :page="page" />
    </div>
</template>

<script>
import SideSection from '~/components/organisms/SideSection.vue';
import MainSection from '~/components/organisms/MainSection.vue';
import { ref } from '@vue/reactivity';

export default {
    components: { SideSection, MainSection },
    emits: ['createPage'],
    setup() {
        const page = ref(false);
        const createPage = () => {
            page.value = true;
            console.log('페이지를 생성해주세요.');
        };

        return { page, createPage };
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
