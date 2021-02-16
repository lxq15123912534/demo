<template>
  <div>
    {{msg}}
    <button @click="handleAdd">
      添加
    </button>
  </div>
</template>

<script>
  import store from '@/store'

  export default {
    name: "Info",
    store,
    data() {
      return {
        msg: 'Hello Info'
      }
    },
    methods: {
      handleAdd() {
        console.log('add info')
        store.commit('execute')
      }
    }
  }
</script>

<style scoped>

</style>
