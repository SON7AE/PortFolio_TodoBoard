<template>
    <header class="header">
        <SearchrBar />
        <CreatePageButton>
            <template #label>Add New Page</template>
        </CreatePageButton>
    </header>
</template>

<script>
import SearchrBar from '../../atoms/SearchrBar.vue';
import CreatePageButton from '../../atoms/CreatePageButton.vue';

export default { components: { SearchrBar, CreatePageButton } };
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.header {
    display: flex;
    flex-direction: column;
    gap: 12px;
}
</style>
