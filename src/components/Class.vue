<template>
    <div>
        <h1 class="classstyle">Class and Style Bindings</h1>
        <h1 v-bind:style="{color:'blue'}">Style Bindings</h1>
        <h1 v-bind:style="{color:colorkey}">Style Bindings with object</h1>
        <h1 v-bind:class="{display:show}">Class Bindings with object</h1>
        <h1 v-bind:class="[aclass]">Class Bindings with Array</h1>              
        <!-- <h1 v-bind:class="['arrayclass']">Class Bindings with Array</h1> -->
        <h1 v-bind:class="[show?'yesshow':'noshow']">Class Bindings with Array</h1>              

    </div>
</template>
<script>
export default {
    name: "Class",
    data(){
        return{
            show:false,
            colorkey:'red',
            aclass:'arrayclass'
        }
    }
}
</script>

<style scoped>
.classstyle{
    color :orange
}
.display{
    background-color: brown;
}
.arrayclass{
    color: cyan;
}
.yesshow{
    background-color:darkorchid;
}
.noshow{
    background-color:deeppink;
}
</style>