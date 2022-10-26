<template>

    <div>
        <h1>this lecture is about watcher</h1>
        <input type="text" v-model="message"/>
        <p v-if="typing">Typing</p><br><br>
        GB:<input type="number" v-model.number="gb">
        MB:<input type="number" v-model.number="mb">
    </div>
</template>
<script>
    export default{
        name:"watcherLec",
        data(){
            return{
                message:'',
                typing:true,
                gb:null,
                mb:null,
            }
        },
        watch:{
            message(newVal,oldVal){
                this.typing=true;
                setTimeout(()=>{
                    this.typing=false;
                },3000);
                console.log("new value:",newVal),
                console.log("old value:",oldVal)
            },
            gb(value){
                this.mb=value*1024;

            },
            mb(value){
                this.gb=value/1024;
            }
        }
    }
</script>