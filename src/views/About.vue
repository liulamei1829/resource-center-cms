<template>
  <div class="about">
    <Topbar></Topbar>
    <h1 v-bind:id="hid"></h1>
    <Footbar />
  </div>
</template>

<script>
import Topbar from '../components/Topbar'
import Footbar from '../components/Footbar'

export default {
  data () {
    return {
      message: '<span>我是about</span>',
      hid:'qwe'
    }
  },
  // mounted() {
  //   setTimeout(()=>{
  //     this.message='abc'
  //   }, 2e3)
  // },
  components: {
    Topbar,
    Footbar
  }
}
</script>

<style lang="scss">
  .about {}
</style>
