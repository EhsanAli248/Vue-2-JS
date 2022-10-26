<template>
    <div>
    <h1>Data Bindig Lectures</h1>
    <h2>{{message}}</h2>
    <input type="text" v-model="message" ><br><br>
    <h2 style="white-space:pre-line">{{mesasge}}</h2>
    <textarea type="text" v-model="message"></textarea><br><br>
    <input v-model="message" placeholder="type here">
    <p>your message is {{message}}</p><br><br>
    <p style="white-space:pre-line">{{message}}</p>
    <textarea v-model="message" placeholder="type here for multiple lines"/><br><br>
    <input type="checkbox" id="checkbox" v-model="checked"> 
    <label for="checkbox">{{checked}}</label><br><br>
    <input type="radio" id="one" value="one" v-model="message">
    <label for="one" >one</label><br>
    <input type="radio" id="two" value="two" v-model="message">
    <label for="two" >two</label>
    <p>picked:{{mesage}}</p>
</div>
</template>
<script>
    export default{
        name:"dataBinding",
        data(){
            return{
                message:"welcome"
            }

        }
    }
</script>