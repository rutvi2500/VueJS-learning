// Child to Parent data(props) transfer

<template>
    <div>
        <h1></h1>
        <!-- <h3>{{name}}</h3> -->
        <button v-on:click="updatetitle">update parent title</button>
    </div>
</template>

<script>
export default {
    name: 'Child',
    methods:{
        updatetitle(){
            //console.warn("Hello from title")
            this.$emit('changetitle','Parent updated')
        }
    }
}
</script>