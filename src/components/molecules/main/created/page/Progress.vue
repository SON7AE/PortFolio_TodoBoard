<template>
    <div class="progress">
        <span class="progress__text">0/0 Completed</span>
        <div class="progress__bar">
            <span></span>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '~/assets/scss/main.scss';

.progress {
    display: flex;
    align-items: center;
    gap: 12px;

    &__text {
        font-family: 'Roboto', sans-serif;
        color: #6d6d6d;
    }
    &__bar {
        width: 238px;
        height: 6px;

        background: #f0f0f0;
        border: 1px solid #e6e6e6;
        border-radius: 3px;
    }
}
</style>
