<template>
    <div>
        <h1>information about props</h1>
        <!-- <h1>{{name}}</h1> -->
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
        name:"propsLec",
        props:['user']
        
    
    }
</script>