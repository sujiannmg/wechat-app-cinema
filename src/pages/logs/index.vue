<template>
  <div class="followRecords">
    <i-button @click="handleClick">默认按钮</i-button>
    <i-button @click="handleClick" type="error" long="true">联通两边按钮</i-button>
    <i-button @click="handleClick" type="primary">Primary</i-button>
    <i-button @click="handleClick" type="ghost">Ghost</i-button>
    <i-button @click="handleClick" type="info">Info</i-button>
    <i-button @click="handleClick" type="success">Success</i-button>
    <i-button @click="handleClick" type="warning">Warning</i-button>
    <i-button @click="handleClick" type="error">Error</i-button>
  </div>
</template>
<script>
  export default {
    name: 'followRecords',
    data () {
      return {
      }
    },
    mounted () {
    },
    methods: {
      handleClick(e) {
        console.log(e);
      }
    }
  }
</script>
<style lang="scss">
  .followRecords {
  }
</style>