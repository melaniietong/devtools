<template>
  <menu class="flex flex-col gap-3 h-full w-full font-sans font-semibold text-white overflow-y-scroll no-scrollbar">
    <ul
      v-for="category in categories"
      :key="category.name"
      :class="`flex flew-row gap-5 align-center p-4 ${category.color} rounded-md`"
    >
      <img
        :src="require('./../../assets/images/icons/' + category.icon + '.svg')"
        class="aspect-square w-6 fill-current text-red-600"
      />
      <div>{{ category.name }}</div>
    </ul>
  </menu>
</template>

<script>
import listOfCategories from './../../data/categories.js'

export default {
  name: 'SideMenu',
  data() {
    return {
      categories: listOfCategories
    }
  }
}
</script>
