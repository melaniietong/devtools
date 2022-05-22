<template>
  <div
    v-for="(post, key) in posts" 
    :key="key"
    class="flex flex-row justify-center w-full p-8"
  >
    <PostContainer
      :num="key"
      :name="post.name"
      :url="post.url"
      :desc="post.desc"
      :category="post.category"
    />
  </div>
</template>

<script>
import listOfPosts from './../../data/data.json'
import PostContainer from './PostContainer.vue'

export default {
  name: 'PostsContainer',
  components: {
    PostContainer
  },
  data() {
    return {
      posts: listOfPosts
    }
  }
}
</script>
