<template>
  <div class="px-16 py-8 fixed top-0 left-0 h-full w-96 bg-white flex flex-col gap-8">
    <h1 class="font-sans text-4xl font-bold text-indigo-700 whitespace-nowrap flex justify-center">devtools</h1>
    <SideMenu />
  </div>
</template>

<script>
import SideMenu from './SideMenu.vue'

export default {
  name: 'SideBar',
  components: {
    SideMenu
  }
}
</script>
