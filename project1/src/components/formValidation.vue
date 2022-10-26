<template>
    <div>
        <p v-if="errors.length">
        <b>Please correct the following errors</b>
        <ul>
            <li v-for="e in errors" v-bind:key="e.id">
                {{e}}

            </li>
        </ul>
        </p>
        <form @submit="login">
            <input type="text" placeholder="Enter your Name" v-model="name"> <br><br>
            <input type="password" placeholder="Enter your Password" v-model="password"><br><br>
            <button type="Submit">Login</button>
        </form>
    </div>
</template>
<script>
    export default{
        name:"formValidation",
        data(){
            return{
                errors:[],
                name:'',
                password:'',
            }
        },methods:{
            login(e)
            {
                this.errors=[];
                if(this.name && this.password){
                    console.warn("All Ok")
                }
                if(!this.name){
                this.errors.push("Name is required")
                }
                if(!this.password){
                    this.errors.push("Password is required")
                }
                console.warn("Hello",this.errors)
                e.preventDefault();
            }
        }

    }
</script>