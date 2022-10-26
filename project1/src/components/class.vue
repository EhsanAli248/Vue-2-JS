<template>
  <div>
    <h1 class="mystyle">This lectures is about class and style</h1>
    <h1 v-bind:style="{color:blue}">style binding</h1>
    <h1 v-bind:style="{color:colorval}">style binding</h1>
    <h1 v-bind:style="styleobject">binding through object directly</h1>
    <h1 v-bind:class="{display:true}">class binding with object</h1>
    <h1 v-bind:class="{display:show}">class binding with object</h1>
    <h1 v-bind:class="['arrayclass']">class binding with array</h1>
    <h1 v-bind:class="[aclass]">class binding with array</h1>
    <h1 v-bind:class="['arrayclass','arrayclass1']">class binding with multiple class</h1>
  </div>  
</template>
<script>
    export default {
        name:"classComp",
        data(){
            return{
                show:true,
                aclass:'arrayclass',
                colorval:'green',
                styleobject:{
                color:'red',
                fontSize:'30px',
                backgroundColor:'yellow'

            }

            };
            
           
        }

    }
    
</script>
<style>
    .mystyle{
        color: brown;
    }
    .display{
        background-color: chartreuse;
    }
    .arrayclass{
        color: aqua;
        background-color: darkgoldenrod;
    }
    .arrayclass1{
        color:brown;
        background-color: rgb(11, 103, 184);
    }
</style>