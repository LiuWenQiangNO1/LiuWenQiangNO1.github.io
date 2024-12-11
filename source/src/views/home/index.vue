<template>
  <div>
    <p>主页</p>
    <button @click="onClickBtn">点击</button>
  </div>
</template>

<script setup lang="ts">
import { useRouter } from "vue-router";

const router = useRouter();
const onClickBtn = () => {
  router.push({
    path: "/user",
    query: {
      id: 111,
    },
  });
};
</script>

<style scoped></style>
