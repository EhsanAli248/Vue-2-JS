<template>
    <div>
    <h1>Hello From Home Component</h1>
    <table border="1px">
        <tr>
            <td>Id</td>
            <td>Name</td>
            <td>Class</td>
        </tr>
        <tr v-for="item in user" :key="item.id">
            <td>{{item.id}}</td>
            <td>{{item.Name}}</td>
            <td>{{item.class}}</td>
        </tr>
    </table>
    
    </div>
</template>
<script>
export default{
        name:"ForLoop",
         
        data(){
        return{
            user:[
                {id:1,Name:"Ehsan",class:10},
                {id:2,Name:"Imran",class:11},
                {id:3,Name:"Salman",class:12}
            ]
        }
    }
        }
</script>

    
