<template>
    <div>
        <h1>Before Mount and Mounted in Life Cycle hook in VueJS</h1>
        <h1>{{name}}</h1>
        <h1 id="demo">{{name}}</h1>

    </div>
</template>
<script>

export default {
    name: 'Login',
    data()
    {
        return{
            name:'rutvi patel'
        }
    },  
    beforeMount()
    {
        //console.warn("before mounted")
        console.warn("before mount",document.getElementById("demo"))                          //Sel defines HTML elements

    },
    mounted()
    {
        //console.warn("mounted")
        console.warn("mounted",document.getElementById("demo"))                          //Sel defines HTML elements
    }
    
}
</script>
