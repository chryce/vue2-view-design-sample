<template>
    <div>
        <child31></child31>
    </div>
</template>

<script>
import child31 from '../../components/child31'

export default {
  name: 'page3_1',
  components: { child31 },
  methods: {
    fatherMethod () {
      console.log('测试3-1')
    }
  }
}
</script>

<style scoped>

</style>
