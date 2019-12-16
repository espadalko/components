<template>
  <div id="app" class="container">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <header class="header">
      <div class="header__title">
        <h1> MenuFix </h1>
      </div>
      <div class="header__menu">
        <MenuFix />
      </div>
    </header>
  
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import MenuFix from './components/MenuFix.vue'

export default {
  name: 'app',
  components: {
    // HelloWorld
    MenuFix
  }
}
</script>

<style lang="stylus">

*
  box-sizing border-box
  margin 0

#app
  border solid 1px grey
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  color #2c3e50

.container
  margin 0 auto
  padding 15px
  height 2000px
  width 700px

.header
  // height 200px
  padding 15px
  background-color grey
  &__title
    height 100px

</style>
