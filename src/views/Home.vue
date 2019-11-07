<template>
  <div class="home">
    <div class="home">
    
    <div class="row">
      <div class="col-md-6">

    <developersProfile v-bind:image = "require('../assets/toothlogo1.png')" v-bind:name="'Tootbook'"></developersProfile>
 </div>

    <div class="col-md-5">
       
      <div class="loginPage"> 
          <div class="container">
            <div class="card">
               <div class="card-header">LOGIN</div>
              
              <div class="card-body">
                <div class="form-group">
                  <label for="username" class="bmd-label-floating">Username</label>
                  <input
                    type="text"
                    class="form-control"
                    id="username"
                    v-model="email"
                    placeholder="Enter username..."
                    required
                  >
                </div>
                <div class="form-group">
                  <label for="pwd" class="bmd-label-floating">Password</label>
                  <input
                    type="password"
                    class="form-control"
                    id="passw"
                    v-model="password"
                    placeholder="Enter password..."
                  >
                </div>
                <center>
                  <button
                    type="button"
                    class="btn btn-outline-success login-btn"
                    id="btnLogin"
                    @click="submit"
                  >Login</button>
                </center>
              </div>
              </div>
            </div>
          </div>
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
  }
};
</script>

<style>
h5{
	color: black;
	margin-left:25%;
	margin-right:25%

}
</style>
