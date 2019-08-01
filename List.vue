<template>
  <div class="list-container">
    <div v-for="(item, index) in data" :key="index">
      <div>{{ item.title }}</div>
      <List v-if="item.children" :data="item.children"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'List',
  props: {
    data: {
      type: Array,
      default: () => []
    }
  }
}
</script>

<style>
.list-container {
  margin-left: 10px
}
</style>