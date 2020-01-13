<template>
  <c-t-login>
    <div slot="lEsquerdo">
      <img src="https://www.designerd.com.br/wp-content/uploads/2013/06/criar-rede-social.png" class="responsive-img">
    </div>
    <div slot="forms" class="card-panel grey lighten-5 z-depth-1">
      <span v-if="!cadastro">
        <h2>Login</h2>
       
          <label for="email">Email:</label>
          <input type="email" name="email" id="email">
          <label for="password">Senha:</label>
          <input type="password" name="password" id="password">
          <button class="btn">Entrar</button>
           <button class="btn orange" v-on:click=" cadastro = !cadastro">Cadatra-se</button>
       
      </span>
      <span v-if="cadastro">
        <h2>Cadastrar</h2>
       
          <label for="nome">Nome:</label>
          <input type="text" name="nome" id="nome">
          <label for="email">Email:</label>
          <input type="email" name="email" id="email">
          <label for="password">Senha:</label>
          <input type="password" name="password" id="password">
          <button class="btn">Cadastrar</button>
          <button class="btn orange" v-on:click=" cadastro = !cadastro">Loga-se</button>
        
      </span>
    </div>
  </c-t-login>
</template>

<script>
import CTLogin from '@/templates/CTLogin'
import CGrid from '@/components/layout/CGrid'
export default {
  name: 'Login',
  components: {
    CTLogin,
    CGrid
  },
  data () {
    return {
      cadastro: false
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
