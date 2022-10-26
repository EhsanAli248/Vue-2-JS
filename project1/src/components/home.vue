 <template>
    <div>
   
     <h2 v-if="show"> conditiional rendering in IF statement</h2>
    <h2 v-else> conditiional rendering in ELSE statement</h2> 
    <button v-on:click="display()">Toggle Button</button>
    <h2>{{data}}</h2>
    <h2>{{msg}}</h2>
    <button v-on:click="hello()">Hello Function</button>
    <!-- <Forloop/> -->
    </div>
    
    </template>
             
<script> 
// import Forloop from '../components/Forloop.vue'
    export default{
        name:"homeComp",
        components:{
            // Forloop
        },
        props:[
            'data',
            'msg'
    ],
    methods:{
        hello()
        {
            alert("Welcome to Hello Function")
            console.log("Hello welcome to console")
        },
    display(){
        this.show=!this.show
    }
    },
    data(){
        return {show:true}
    }
  

   
}
            
    
    
</script>