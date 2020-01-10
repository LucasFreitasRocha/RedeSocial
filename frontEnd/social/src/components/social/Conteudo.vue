<template>
<div class="row">
  <div class="card ">
    <div class="card-content white-text">
      <span class="card-title">
        <div class="row valign-wrapper">
          <c-grid tamanho="2">
              <img :src="fotoPerfil" alt="" class="circle responsive-img">
              <!-- notice the "circle" class -->
          </c-grid>
          <c-grid tamanho="10">
              <span class="black-text">
                  <strong>{{nome}}</strong> - <small>{{data}}</small>
              </span>
          </c-grid>
        </div>

      </span>

      <publicacao img="https://wallpaperaccess.com/full/1901974.jpg"
      title="#tbt"  txt="Eu novinho"/>

    </div>
    <div class="card-action">
      <p>
          <i class="material-icons">favorite_border</i>
          <i class="material-icons">insert_comment</i>
      </p>
    </div>
  </div>
</div>
</template>

<script>
import CGrid from '@/components/layout/CGrid'
import Publicacao from '@/components/social/Publicacao'
export default {
  name: 'Conteudo',
  props: ['fotoPerfil', 'nome', 'data'],
  components: {
    CGrid,
    Publicacao
  },
  data () {
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 p{
   color: black;
 }
</style>
