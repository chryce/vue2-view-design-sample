<template>
    <ul id="example-1">
        <li v-for="item in items" :key="item.message">
            {{ item.message }}
        </li>
    </ul>
</template>

<script>
export default {
  name: 'page1',
  data: function () {
    return {
      items: [
        { message: 'Page1----A' },
        { message: 'Page1----B' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
