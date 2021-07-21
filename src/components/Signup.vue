// Form with Checkbox and Radio Button in VueJS
// Validation

<template>
    <div>
        <p v-if="error.length">
            <b>Please correct following errors:</b>
            <ul>
                <li v-for="e in error" v-bind:key="e.id">
                    {{e}}
                </li>
            </ul>    
        </p>
        <h1>Form with Validation in VueJS</h1>
        <input type="text" placeholder="Enter your name" v-model="username" /><br><br>
        <input type="text" placeholder="Enter your password" v-model="password" /><br><br>
        <input type="checkbox" id="cricket" value="cricket" v-model="hobbies"/>
        <label for="cricket">Cricket</label>
        <input type="checkbox" id="football" value="football" v-model="hobbies"/>
        <label for="football">football</label><br><br>
        <input type="radio" id="male" value="male" v-model="gender"/>
        <label for="male">male</label>
        <input type="radio" id="female" value="female" v-model="gender"/>
        <label for="female">female</label><br><br>
        <button v-on:click="signupUser">Sign Up</button>
    </div>
</template>

<script>
export default {
    name: 'Signup',
    data(){
        return{
            error:[],
            signup:{
                username:null,
                password:null,
                hobbies:[],
                gender:null
            }
        }
    },
    methods:{
        signupUser(e)
        {
            this.error=[];
            if(this.username && this.password)
            {
                console.warn("no error")
            }
            if(!this.username)
            {
                this.error.push("Username is required");
            }
            if(!this.password)
            {
                this.error.push("Password is required");
            }
            if(!this.hobbies)
            {
                this.error.push("Please select atleast one hobby");
            }
            if(!this.gender)
            {
                this.error.push("Gender is required");
            }
            console.warn(this.signup, this.error);
            e.preventDefault()                      //form won't reload
        }
    }
}
</script>