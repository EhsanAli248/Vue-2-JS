<template>
    <div>
        <h3 id="demo">{{name}}</h3>
    </div>
</template>
<script>
    export default{
        name:"lifeCycle2",
        data(){
            return{
                name:"Ehsan Ali",
            }
        },
        beforeMount(){
            // console.warn("before mount is called",this.$el)
            // console.warn("before mounted",document.getElementById("demo"))
        },
        mounted(){
            console.warn("Mounted is called",this.$el)
            // console.warn("Mounted",document.getElementById("demo"))
        }

    }
</script>