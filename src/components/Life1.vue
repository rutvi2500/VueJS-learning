<template>
    <div>
        <h1>Before Create and Created in Life Cycle of VueJS</h1>
        <h1>{{name}}</h1>
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
    created()
    {
        //this.name="Root"
        console.warn("created", this.name)
    },
    beforeCreate()
    {
        this.name="Root"                                //name will not change because object has not been created yet. So, for while it will be changed and then data will be called afterwards, So, it will again set the name as per the data.
        console.warn("before", this.name)
    },
    
    
}
</script>
