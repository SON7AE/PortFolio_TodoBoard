<template>
    <button class="button-basic">
        {{ data }}
    </button>
</template>

<script>
export default {
    props: {
        data: {
            type: String,
            required: true,
        },
    },
};
</script>

<style></style>
