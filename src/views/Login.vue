<template>
<div>

<center><h2> ADMIN</h2></center>
<div id="placement" class="row">
<div class="col-md-5">
    <developersProfile v-bind:image = "require('../assets/toothlogo1.png')" v-bind:name="'Tootbook'"></developersProfile>
</div>
<div class= "col-md-6">

    <div id="login">
        <center><h1>Login</h1></center>
        <div class="form-group">
                  <label for="formGroupExampleInput" class="bmd-label-floating">Username</label>
                  <div>
        <input type="text" name="username" v-model="input.username" placeholder="Enter username" />
        </div>
        </div>
        <div class="form-group">
                    <label for="formGroupExampleInput2" class="bmd-label-floating">Password</label>
                  <div>
        <input type="password" name="password" v-model="input.password" placeholder="Enter password" />
        </div>
         </div>
         <center>
        <button type="button"   class="btn btn-outline-info login-btn" v-on:click="login()">Login</button>
        </center>
    </div>
    </div>
     
     </div>
     </div>
</template>

<script>
import developersProfile from "../components/developersProfile";
    export default {
        components:{
    developersProfile
  },
        name: 'Login',
        data() {
            return {
                input: {
                    username: "",
                    password: ""
                }
            }
        },
        methods: {
            login() {
                if(this.input.username != "" && this.input.password != "") {
                    if(this.input.username == this.$parent.mockAccount.username && this.input.password == this.$parent.mockAccount.password) {
                        this.$emit("authenticated", true);
                        this.$router.replace({ name: "home" });
                    } else {
                        // console.log("The username and / or password is incorrect");
                    }
                } else {
                    // console.log("A username and password must be present");
                }
            }
        }
    }
</script>

<style scoped>
    #login {
        width: 500px;
        border: 1px solid #CCCCCC;
        background-color:skyblue;
        margin: auto;
        margin-top: 100px;
        padding: 50px;
        
    }

    button{
        margin-top:50px;
        background-color: black;
        width: 200px;
    }

    #placement{
        margin-left:10%;
    }

    h2{
        font-family: 'Lucida Sans';
        font-size: 80px;
        color:black;
    }
</style>