<template>
  <c-main>
    <publicar/>
    <contuedo fotoPerfil="https://vignette.wikia.nocookie.net/pt.starwars/images/6/6c/2511.jpg/revision/latest?cb=20121107230903"
    nome="Yoda"
    data="10/01/2020 - 16:09"/>
  </c-main>

</template>

<script>
import CMain from '@/templates/CMain'
import Contuedo from '@/components/social/Conteudo'
import Publicar from '@/components/social/Publicar'
export default {
  name: 'Home',
  components: {
    Contuedo,
    Publicar,
    CMain
  },
  data () {
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
