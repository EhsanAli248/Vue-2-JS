<template>
    <div>
        <h3>{{name}}</h3>
    </div>
</template>
<script>
    export default{
        name:"lifeCycle1",
        data(){
            return{
                name:"Ehsan Ali"
            }
        },
        
        beforeCreate(){
            // this.name="Ali Baba"
            console.warn("before created call")
            // console.warn("before created call",this.name)
        },
        created(){
            console.warn("created is called")
            // console.warn("created is called",this.name)
        },
        // created(){
        //     console.warn("created is called")
        // }
         

        
    }
</script>