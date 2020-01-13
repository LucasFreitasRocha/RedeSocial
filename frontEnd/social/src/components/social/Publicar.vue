<template>
    <div class="row">
        <c-grid class="input-field" tamanho="12">
          <textarea id="publicar" v-model= "conteudo" class="materialize-textarea"></textarea>
          <label for="publicar">Fala pra Nós</label>
        </c-grid>
        <p>
          <c-grid  v-if= "conteudo" class=" btn waves-effect waves-light" tamanho="2 offset-s10">
          Publicar</c-grid>
        </p>
    </div>
</template>

<script>
import CGrid from '@/components/layout/CGrid'
export default {
  name: 'Publicar',
  props: ['img', 'title', 'txt'],
  components: {
    CGrid
  },

  data () {
    return {
      conteudo: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 p{
   color: black;
 }
</style>
