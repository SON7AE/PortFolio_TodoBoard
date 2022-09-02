<template>
  <h1>Home.vue 컴포넌트 입니다.</h1>
  <ButtonBasic :data="'Add New Page'" />
</template>

<script>
import ButtonBasic from '../components/atoms/ButtonBasic.vue';
export default {
  components: { ButtonBasic },
};
</script>

<style></style>
