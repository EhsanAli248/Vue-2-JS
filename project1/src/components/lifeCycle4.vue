<template>
    <div>
        <h2 ref="count">{{count}}</h2>
        <button @click="count++">update </button>
    </div>
</template>
<script>
    export default{
        name:"lifeCycle4",
    
    data(){
        return{
            count:0,
        }

    },
    beforeUpdate() {
        console.warn("before updated",this.$refs['count'].textContent);
    },
    updated(){
        console.warn("updated", this.$refs['count'].textContents);
    }
}
</script>