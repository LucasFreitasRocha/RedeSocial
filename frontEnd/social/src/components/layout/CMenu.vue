<template>
<div class="card-panel grey lighten-5 z-depth-1">
    <div class="row valign-wrapper">
        <c-grid tamanho="4">
            <img src="https://vignette.wikia.nocookie.net/pt.starwars/images/6/6c/2511.jpg/revision/latest?cb=20121107230903" alt="" class="circle responsive-img">
            <!-- notice the "circle" class -->
        </c-grid>
        <c-grid tamanho="8">
            <span class="black-text">
                <h5>Maria Silva</h5>
                This is a square image. Add the "circle" class to it to make it
                appear circular.
            </span>
        </c-grid>
    </div>
</div>
</template>

<script>
import CGrid from '@/components/layout/CGrid'
export default {
  name: 'CMenu',
  components: {
    CGrid
  },
  data () {
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
