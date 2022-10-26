<template>
    <div>
        <h1>Props:Child to Parent</h1>
        <button v-on:click="updatefun()">Update text </button>
    </div>
</template>
<script>
    export default{
        name:"propsLec1",
        methods:{
            updatefun(){
                this.$emit('changeTitle',"parent updated");
            }
        }
    }
</script>