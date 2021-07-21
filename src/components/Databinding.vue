<template>
    <div>
        <h1>Data Binding in VueJS</h1>
        <h1>{{message}}</h1>
        <h2 style="white-space:pre-line">{{address}}</h2>
        <input text type="text" v-model="message"><br><br><br>
        <textarea type="text" v-model="address" />
    </div>
</template>

<script>
export default {     
    name:'Databinding',
    data(){
        return{
            message:"Hi",
            address:"hey there"
        }
    }
}
</script>