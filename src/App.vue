<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

</script>


<template>
  <ElContainer class="outer-c">
    <ElHeader class="header">xxx</ElHeader>
    <ElContainer class="inner-c">
      <ElAside width="240px" class="aside">
        <!-- <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink> -->
        <ElMenu router>
          <ElSubMenu index="1">
            <template #title>
              <div>主页信息</div>
            </template>
            <ElMenuItem index="/">Home</ElMenuItem>
            <ElMenuItem index="/about">About</ElMenuItem>
          </ElSubMenu>
          <ElSubMenu index="2">
            <template #title>
              <div>基础资料</div>
            </template>
            <ElMenuItem index="/material">物品信息</ElMenuItem>
            <ElMenuItem index="/xx">物品信息xx </ElMenuItem>
          </ElSubMenu>
        </ElMenu>
      </ElAside>
      <ElMain class="main">
        <RouterView />
      </ElMain>
    </ElContainer>
  </ElContainer>
</template>

<style scoped>
.outer-c {
  height: 100vh;
}
.inner-c {
  border: solid 1px rebeccapurple;
}
.header{
  background-color: burlywood;
}
.aside{
  background-color: burlywood;
}
</style>