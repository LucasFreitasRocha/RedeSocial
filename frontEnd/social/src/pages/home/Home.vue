<template>
  <span>
    <div class="row">
        <div class="input-field col s12">
          <textarea id="textarea1" class="materialize-textarea"></textarea>
          <label for="textarea1">Fala pra Nós</label>
        </div>
        <p>
          <button class=" btn waves-effect waves-light col s2 offset-s10">Publicar</button>
        </p>
    </div>

    <contuedo fotoPerfil="https://vignette.wikia.nocookie.net/pt.starwars/images/6/6c/2511.jpg/revision/latest?cb=20121107230903"
    nome="Yoda"
    data="10/01/2020 - 16:09"/>
  </span>

</template>

<script>
import Contuedo from '@/components/social/Conteudo'
export default {
  name: 'Home',
  components: {
    Contuedo
  },
  data () {
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
