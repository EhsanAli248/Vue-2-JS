<template>
    <div>
            
            <p>Normal message:{{message}}</p><br>
            <p>Reversed message:{{reversemsg}}</p>
    </div>
</template>
<script>
    export default{
        name:"computedPrp",
        data(){
            return{
                // message:"Hello",
                message:'Ehsan Ali',
            }
        },
        computed:{
            reversemsg(){
                return this.message.split('').reverse().join('')
                

            }
        }
    }
</script>