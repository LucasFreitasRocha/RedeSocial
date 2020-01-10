<template>
  <div id="app">
    <header>
      <nav-bar logo="social"/>
    </header>
    <main class="container">
      <div class="row">
        <c-grid tamanho="4"> <c-menu/> </c-grid>
        <c-grid tamanho="8">
            <router-view/>
        </c-grid>

      </div>
    </main>

    <c-footer>
      <li><a class="grey-text text-lighten-3" href="#!">teste</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
      <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
    </c-footer>
  </div>
</template>

<script>
import NavBar from '@/components/layout/NavBar'
import CFooter from '@/components/layout/CFooter'
import CGrid from '@/components/layout/CGrid'
import CMenu from '@/components/layout/CMenu'
export default {
  name: 'App',
  components: {
    NavBar,
    CFooter,
    CGrid,
    CMenu
  }
}
</script>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
nav{
  text-align: left;
}
</style>
