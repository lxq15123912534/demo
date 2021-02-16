<template>
  <div class="about">
    <h1>This is an about page</h1>
    <h2>
      {{stateCount}}
    </h2>
  </div>
</template>
<script>
  import store from '@/store'

  export default {
    name: 'about',
    store,
    data() {
      return {
        stateCount: store.state.count
      }
    }
  }
</script>
