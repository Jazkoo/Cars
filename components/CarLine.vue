<!-- Please remove this file from your project -->
<template>
  <div class="card" :style="{'background-image':'url('+ image +')'}"">
  
    <div class="text-content">
      <h2>{{name}}</h2> 
      <table cellpadding="0" cellmargin="0"> <tr v-for="(feature,key) in features"> <td>{{feature.title}}</td> <td>{{feature.value}}</td> </tr> </table>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CarLine',
  props:{
    name:{required:true},
    image:{required:false},
    features:{required:false}
    }
}

</script>
<style>
  .card{
    width: 55%;
    position: relative;
    background: black;
    margin: 20px;
    height: 500px;
    background-size:cover
  }
  .image{
    position:absolute;
    height:500px;
    overflow:hidden;
    z-index:1;
  }
  img{
     max-width:100%;
     background-size:cover;
     background-position:center;
  }
  .text-content{
    padding-top:50px;
    position:relative;
    z-index:2;
        padding:20px;

  }

</style>
