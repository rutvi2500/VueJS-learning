<template>
    <div>
        <h1>Hello from Home Component</h1>
        <h2>{{msg}}</h2>
        <!-- if else -->
        <h1 v-if="show">Condition Rendering in Vue</h1>
        <h1 v-else>Condition Rendering else block</h1>
        <button v-on:click="display">Toggle Element</button><br><br><br>
        <!-- <h2>{{data}}</h2>
        <h2>{{msg}}</h2> -->
        <button v-on:mouseover="hello('hello call')">Call Hello Function</button>
        <h1>For loop in vuejs</h1>
        <table border="1px">
            <tr>
                <td>Id</td>
                <td>Name</td>
                <td>Email</td>
            </tr>
            <tr v-for="user in users" :key="user.id">
                <td>{{user.id}}</td>
                <td>{{user.name}}</td>
                <td>{{user.email}}</td>
            </tr>
        </table>
    </div>
</template>
<script>
export default {
    name: 'Basic',
    props:{
        data:String,
        msg:String
    },
    data(){                                             
        //return {show:false}                          // for if-else condition
        return{
            show:false,                         // for if-else condition
            users:[                             // for loop
                {id:1,name:'peter',email:'peter@test.com'},
                {id:2,name:'abc',email:'abc@test.com'},
                {id:3,name:'pqr',email:'pqr@test.com'},
                {id:4,name:'xyz',email:'xyz@test.com'},
            ]
        }
    },methods:{
        hello(data)
        {
            alert(data)
            console.log("Hello Console")
        },
        display()
        {
            this.show=!(this.show)              //it will help to toggle. Eg. hidden--> show and Shown--->hidden
        }
    }
}
</script>
