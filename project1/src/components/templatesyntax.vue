<template>
    <div>
        <h1 v-html="rawhtml"></h1>
    <h1>This page tells you about diifferent HTML synatx in Vue Js</h1>
    <h3>{{name}}</h3>
    <h3 v-once>{{name}}</h3>
    <h3>{{a+b}}</h3>
    <h3>{{ok?"yes":"No"}}</h3>
    <button v-on:click="updatetax">Click Button</button>
    <!-- <button v-bind:disabled="disablebtn" v-on:click="updatetax">Click Button</button> -->
    
    </div>
</template>

<script>
    export default{
        name:"templateSyntax",
      data(){
        return {
            name:'Ehsan',
            a:20,
            b:30,
            ok:true,
            rawhtml:"<h1>This is my HTML</h1>", 
            disablebtn:false
        }
    },methods:{
        updatetax()
        {
            this.name='Ali'
            this.ok=!this.ok
        }
    }
    }
</script>