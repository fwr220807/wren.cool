<script setup lang="ts">
const route = useRoute()
const inactiveStyle = 'opacity-20 hover:opacity-50'
</script>

<template>
  <div mb-0 flex="~ gap5 sm:gap6 wrap" items-center text-xl sm:text-3xl select-none>
    <router-link to="/posts" class="!border-none !font-400" decoration-none :class="route.path === '/posts' ? '' : inactiveStyle">
      Blog
    </router-link>
    <router-link to="/diary" class="!border-none !font-400" decoration-none :class="route.path === '/diary' ? '' : inactiveStyle">
      Diary
    </router-link>
    <router-link to="/algorithm" class="!border-none !font-400" decoration-none :class="route.path === '/algorithm' ? '' : inactiveStyle">
      Algo
    </router-link>
  </div>
</template>
