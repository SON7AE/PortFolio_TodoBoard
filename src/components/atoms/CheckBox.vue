<template>
    <div class="round">
        <input type="checkbox" id="checkbox" />
        <label for="checkbox"></label>
    </div>
</template>

<script>
export default {};
</script>

<style>
.round {
    position: relative;
}

.round label {
    width: 24px;
    height: 24px;

    background-color: #fff;
    border: 2px solid #e4e4e4;
    border-radius: 6px;
    cursor: pointer;

    position: absolute;
    top: -5px;
    left: 0;
}

.round label:after {
    width: 12px;
    height: 6px;

    border: 2px solid #fff;
    border-top: none;
    border-right: none;
    content: '';

    position: absolute;
    top: 6px;
    left: 6px;

    transform: rotate(-45deg);
    opacity: 0;
}

.round input[type='checkbox'] {
    visibility: hidden;
}

.round input[type='checkbox']:checked + label {
    background-color: #00f38d;
    border-color: #00f38d;
    border-radius: 50%;
    transition: 0.2s ease-in-out;
}

.round input[type='checkbox']:checked + label:after {
    opacity: 1;
}
</style>
