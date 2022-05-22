<template>
  <div class="h-full w-full ml-96">
    <PostsContainer />
  </div>
</template>

<script>
import PostsContainer from './Posts/PostsContainer.vue'

export default {
  name: 'MainBody',
  components: {
    PostsContainer
  }
}
</script>
