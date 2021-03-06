<template>
  <div id="app">
    <div class="flex bg-gray-100 border-b border-gray-300 py-4">
        <div class="container mx-auto flex justify-between">
            <div class="a">
                <router-link to='/About'>About</router-link>
            </div>
            <div class="b">
                <router-link class="mr-4" to='/Login' exact>Login</router-link>
                <router-link to='/Register'>Register</router-link>
            </div>
        </div>
        <hr style="border-width: 3px;">
    </div>
    <div class="container mx-auto py-2">
        <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
div.a{
  text-align: left;
  font-size: 20px;
  margin-top: -35px;
}

div.b{
  text-align: right;
  font-size: 20px;
  margin-top: -25px;
}
</style>
