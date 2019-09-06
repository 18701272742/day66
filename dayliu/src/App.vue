<template>
  <div id="app">
    <div class="top">
      <router-view/>
    </div>
    <div id="nav">
      <router-link to="/">首页</router-link> 
      <router-link to="/about">我的</router-link>
    </div>
    
  </div>
</template>

<style lang="scss">
@import url('./style/style.css');
</style>
