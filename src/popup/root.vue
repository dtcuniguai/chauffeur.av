<template lang="html">
  <div ref="btn" class="el-button el-button--primary" @click="tab">
    <span>New tab</span>
  </div>
</template>
<script>
  import cheerio from 'cheerio'

  export default {
    props: ['display'],
    data: () => ({
      status: 1
    }),
    computed: { },
    watch: {
      display () {

      }
    },
    created () {
      console.log('New tab')
    },
    mounted () { },
    methods: {
      tab () {
        console.log('change')
        console.log(this.$refs['btn'])
        console.log(cheerio)
        // chrome.tabs.create({ url: 'pages/app.html' })
      }
    }
  }
</script>
<style lang="scss">
  div {
    color: blue
  }
</style>
