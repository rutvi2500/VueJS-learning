<template>
    <div>
        <h1>Before Destroy and Destroyed in Life Cycle hook in VueJS</h1>
        <!-- <h1 id="demo">{{name}}</h1> -->

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
    beforeUnmount()
    {
        alert("Hey there!")
        console.warn("before destroy")

    },
    unmounted()
    {
        alert("Hey there!")
        console.warn("destroyed")
    }
    
}
</script>
