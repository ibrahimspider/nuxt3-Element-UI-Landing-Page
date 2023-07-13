<template>
  <el-menu
    :default-active="activeIndex"
    class="el-menu-demo"
    mode="horizontal"
    :ellipsis="false"
    @select="handleSelect"
  >
    <el-menu-item class="logo"><span>Zivaco</span></el-menu-item>
    <div class="flex-grow" />
    <el-menu-item index="1">Home</el-menu-item>
    <el-menu-item index="3">Contact</el-menu-item>
    <el-sub-menu index="4">
      <template #title>user</template>
      <el-menu-item index="4-1">Login</el-menu-item>
      <el-menu-item index="4-2">register</el-menu-item>
      <el-menu-item index="4-3">settings</el-menu-item>
      <el-sub-menu index="4-4">
        <template #title>item four</template>
        <el-menu-item index="4-4-1">item one</el-menu-item>
        <el-menu-item index="4-4-2">item two</el-menu-item>
        <el-menu-item index="4-4-3">item three</el-menu-item>
      </el-sub-menu>
    </el-sub-menu>
  </el-menu>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const activeIndex = ref("1");
const handleSelect = (key: string, keyPath: string[]) => {
  console.log(key, keyPath);
};
</script>

<style scoped>
.el-menu-demo {
  width: 100%;
  overflow: hidden;
}
.flex-grow {
  flex-grow: 1;
}
.logo {
  font-weight: bold;
  font-size: 28px;
}
</style>
