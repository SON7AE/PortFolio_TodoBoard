<template>
    <header class="header">
        <SearchrBar />
        <CreatePageButton @createPage="createPage">
            <template #label>Add New Page</template>
        </CreatePageButton>
    </header>
</template>

<script>
import SearchrBar from '~/components/atoms/SearchrBar.vue';
import CreatePageButton from '~/components/atoms/CreatePageButton.vue';

export default {
    components: { SearchrBar, CreatePageButton },
    emits: ['createPage'],
    setup(props, { emit }) {
        const createPage = () => {
            emit('createPage');
        };

        return {
            createPage,
        };
    },
};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.header {
    display: flex;
    flex-direction: column;
    gap: 12px;
}
</style>
