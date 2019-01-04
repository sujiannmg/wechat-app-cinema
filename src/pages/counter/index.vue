<template>
  <div class="counter-warp">
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
    <p>Vuex counter：{{ count }}</p>
    <p>
      <button @click="increment">+</button>
      <button @click="decrement">-</button>
    </p>
    <a href="/pages/index/main" class="home">去往首页</a>

  </div>
</template>

<script>
// Use Vuex
import store from './store'

export default {
  name: 'followRecords',
  computed: {
    count () {
      return store.state.count
    }
  },
  methods: {
    increment () {
      store.commit('increment')
    },
    decrement () {
      store.commit('decrement')
    },
    handleClick(e) {
      console.log(e);
    }
  }
}
</script>

<style>
.counter-warp {
  text-align: center;
  margin-top: 100px;
}
.home {
  display: inline-block;
  margin: 100px auto;
  padding: 5px 10px;
  color: blue;
  border: 1px solid blue;
}
.followRecords {

}
</style>
