<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <homeComp/> -->
  <!-- <homeComp data="Ehsan is here" msg="Hy from Fluxystem"/> -->
  <!-- <templatesyntax/> -->
  <!-- <homeComp/> -->
  <!-- <Forloop/> -->
  <!-- <classComp/> -->
  <!-- <DataBinding/> -->
  <!-- <propsLec v-bind:user="users"/> -->
  <!-- <h1>{{title}}</h1>
    <propsLec1 v-on:changeTitle="updateTitle($event)"/> -->
    <!-- <formValidation/> -->
    <!-- <lifeCycle1/> -->
    <!-- <lifeCycle2/> -->
    <!-- <lifeCycle3/> -->
    <!-- <watcherLec/> -->
    <!-- <computedPrp/> -->
    <lifeCycle4/>

  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import homeComp from './components/home.vue'
// import Forloop from './components/Forloop.vue'
// import templatesyntax from './components/templatesyntax.vue'
  //  import classComp from './components/class.vue'
// import DataBinding from './components/dataBinding.vue';
  //  import propsLec from './components/propsLec.vue'
  // import propsLec1 from './components/propsLec1.vue'
  // import formValidation from './components/formValidation.vue'
// import lifeCycle1 from './components/lifeCycle1.vue';
// import lifeCycle2 from './components/lifeCycle2.vue';
// import lifeCycle3 from './components/lifeCycle3.vue';
// import watcherLec from './components/watcher.vue';
// import computedPrp from './components/computedPrp.vue';
import lifeCycle4 from './components/lifeCycle4.vue';





export default {
  name: 'App',
  components: {
    // HelloWorld,
    // homeComp,
    // Forloop,
    // templatesyntax
    // classComp,
    // DataBinding
    // propsLec,
    // propsLec1
    // formValidation,
    // lifeCycle1,
    // lifeCycle2,
    // lifeCycle3
    // watcherLec,
    // computedPrp
    lifeCycle4,
},
// data(){
        // return{
            // users:[
            //     {id:1,Name:"Ehsan",class:10},
            //     {id:2,Name:"Imran",class:11},
            //     {id:3,Name:"Salman",class:12}
            // ]
            // title:"props Tutorial"
        // }

    // },
    // methods:{
    //   updateTitle(title){
    //     this.title=title;
    //   }

    // }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
