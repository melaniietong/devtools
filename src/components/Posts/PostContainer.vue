<template>
  <div class="w-4/12">
    <img 
      :src="require('./../../assets/images/screenshots/' + num + '.png')"
    />
    <a :href="url">{{name}}</a>
    {{desc}}
    {{category}}
  </div>
</template>

<script>
export default {
  name: 'PostContainer',
  props: {
    num: String,
    name: String,
    url: String,
    desc: String,
    category: Array
  }
}
</script>
