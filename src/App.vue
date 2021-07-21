<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <!-- <Basic data="Rutvi Here!" msg="Hi Rutvi!"/> -->
    <!-- <Componentmain/> -->
    <!-- <Temp/> -->
    <!-- <Class/> -->
    <!-- <Databinding/> -->
    <!-- <Propchild v-bind:users="users"/> -->

    <!-- <h1>Send Props from child to parent</h1>
    <h1>{{title}}</h1>
    <Propparent v-on:changetitle="updatetitle($event)"/> -->

    <!-- <Signup />     -->

    <!-- // Filter -->
    <!-- <h1>{{(name | Ucase)}}</h1>
    <h1>{{(amount | currencyConverter)}}</h1> -->

    <!-- <Life1/> -->
    <!-- <Life2 /> -->

    <!-- <div v-if="display">
          <Life3 />
    </div>
    <button v-on:click="toggle">Toggle</button> -->


  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import Componentmain from './components/Componentmain.vue'
// import Temp from './components/Temp.vue'
// import Basic from './components/Basic.vue'
// import Databinding from './components/Databinding.vue'
// import Propchild from './components/Propchild.vue'
// import Propparent from './components/Propparent.vue'
// import Signup from './components/Signup.vue'
// import Life1 from './components/Life1.vue';
// import Life3 from './components/Life3.vue'

export default {
  name: "App",
  components: {
    //HelloWorld,
    // Basic
    // Componentmain,
    // Temp
    // Class,
    // Databinding,
    // Propchild,
    // Propparent,
    // Signup
    // Life1
    // Life2
    // Life3
  },
  data()
  {
    // return{users:[                                               //for parent to child prop transfer
    //   {name:"ABC", email:"abc@gmail.com"},
    //   {name:"PQR", email:"pqr@gmail.com"},
    //   {name:"XYZ", email:"xyz@gmail.com"},
    //   ]}

    // return{                                                    // for child to parent prop transfer
    //   title:"props tutorial"
    // }

    //filter
    // return{
    //   name:"rutvi patel",
    //   amount:100
    //}

    //Destroyed & befor destroy
    // return{
    //   display:true
    // }
  },
  // methods:{                                                      // for child to parent prop transfer
  //     updatetitle(title)
  //     {
  //       this.title=title
  //     }
  //   }

  //Distroyed and before destroy
  // methods:{
  //   toggle()
  //   {
  //     this.display=!this.display
  //   }
  // }
};
</script>

<style lang="scss">
@import "~@/assets/scss/vendors/bootstrap-vue/index";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>