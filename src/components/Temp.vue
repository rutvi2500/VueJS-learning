<template>
    <div>
        <p v-html="rowHtml"></p>
        <!-- <h1>Template in vueJS</h1> -->
        <h3 v-once>{{name}}</h3>
        <h3>{{name}}</h3>
        <h3>{{15+15}}</h3>
        <h3>{{a+b}}</h3>
        <h3>{{ok?"Yes":"No"}}</h3>
        <button v-bind:disabled="disablebtn" v-on:click="updatetext">Click Me</button>
    </div>
</template>
<script>
export default {
    name: "Template",
    data(){
        return{
            name: 'Rutvi',
            a:10,
            b:10,
            ok:true,
            rowHtml:"<h1>Template in vueJS</h1>",
            disablebtn:false,
        }
    },
    methods:{
        updatetext(){
            this.name="Peter"
            this.ok=!this.ok
        }
    }
}
</script>
