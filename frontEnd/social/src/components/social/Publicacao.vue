<template>
    <span>
        <div class="card-image">
            <img :src="img || 'https://materializecss.com/images/sample-1.jpg'">
            <div class="card-title"> {{title || ''}} </div>
        </div>
        <div class="card-content ">
            <p>{{txt || ''}}</p>
        </div>
    </span>
</template>

<script>
export default {
  name: 'Publicacao',
  props: ['img', 'title', 'txt'],
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
