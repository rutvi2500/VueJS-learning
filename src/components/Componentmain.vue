<template>
    <div>
        <h1>Home Component</h1>
        <Component1/>
        <Component2/>
        <Component2/>

    </div>
</template>

<script>
import Component1 from './Component1.vue'
import Component2 from './Component2.vue'
export default {
    name:'Componentmain',
    components:{
        Component1,
        Component2
    }

}
</script>

<style scoped>
div{
    background-color: #dde5ec;
    height: 500px;
}

</style>
