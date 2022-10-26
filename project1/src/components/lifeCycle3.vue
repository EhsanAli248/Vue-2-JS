<template>
    <div>
        <div v-if="show">
        <h3>{{name}}</h3></div>
        <!-- <button v-on:click="toggle">Toggle</button> -->
        <button @click="toggle()">Toggle</button>
    </div>
</template>
<script>
    export default{
        name:"lifeCycle3",
        data(){
            return{
                name:"Ehsan Ali",
                show:true
            }
        },methods:{
            toggle(){
                
                this.show=!this.show
            }
        },
        beforeDestroy(){
            console.warn("before destroyed")
        },
        Destroyed(){
            console.warn("destroyed")
        }
        

    }
</script>