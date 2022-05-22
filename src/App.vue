<template>
  <div class="flex flex-row w-full h-full bg-gray-50">
    <SideBar />
    <MainBody />
  </div>
</template>

<script>
import MainBody from './components/MainBody.vue'
import SideBar from './components/SideBar/SideBar.vue'

export default {
  name: 'App',
  components: {
    MainBody, SideBar
  }
}
</script>
