<template>
  <div id="main">
    <header>
      <nav-bar logo="Social">
        <li><router-link to="/"> Home </router-link></li>
        <li><router-link to="/login">Login </router-link></li>
      </nav-bar>
    </header>
    <main class="container">
      <div class="row">
        <c-grid tamanho="4"> <c-menu nome="Yoda Jedi"/> </c-grid>
        <c-grid tamanho="8">
           <slot></slot>
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
  name: 'CMain',
  components: {
    NavBar,
    CFooter,
    CGrid,
    CMenu
  },
  data () {
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
