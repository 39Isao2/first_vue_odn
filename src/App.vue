<template>
  <div id="app">
    <div id="header">
      <router-link to="/">こんにゃく</router-link>
      <router-link to="/page2">煮卵</router-link>
      <router-link to="/page3">ちくわ</router-link>
    </div>
    <router-view></router-view>
  </div>
</template>

<!-- コンポーネントの名前を定義 -->
<script>
export default {
  name: 'App'
}
</script>

<!--スタイルの指定をします-->
<style>
body {
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#header {
  height: 40px;
  background: white;
  box-shadow: 0px 3px 3px rgba(0,0,0,0.1);
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top:50px;
}

#header a {
    text-decoration: none;
    margin: 0 10px;
    padding: 7px;
    background: gray;
    color: #fff;
}
</style>
