<template>
<b-container>
    <b-modal id="loginSignupModal" 
    hide-header
    hide-footer
    no-close-on-backdrop 
    no-close-on-esc
    centered
    v-model="showLoginSignupModal">
        <b-container fluid>
            <b-row>
                <b-col>
                <img src="/static/images/logo.png" float-center>
                <button type="button" class="close" @click="showLoginSignupModal=false" aria-label="Close" style="margin-left:25px;margin-top:0px;" float-right>
                    <span aria-hidden="true">&times;</span>
                </button>
                </b-col>
                
            </b-row>
            <b-row>
                <b-col>
<b-tabs>
  <b-tab title="Login">
      <b-container fluid style="margin-top: 50px;">
          <b-row>
              <b-col>
                <div class="input-group mb-3">
                <div class="input-group-prepend" >
                    <span class="input-group-text" style="border-radius: 50px 0px 0px 50px;">
                      <i class="fa fa-user" aria-hidden="true"></i>
                    </span>
                </div>
                  <input type="text" class="form-control" placeholder="email/mobile number" style="border-radius:  0px 50px 50px 0px;">
                </div>                  
              </b-col>
          </b-row>
          <b-row>
              <b-col>
                <div class="input-group mb-3">
                <div class="input-group-prepend" >
                    <span class="input-group-text" style="border-radius: 50px 0px 0px 50px;"><i class="fa fa-unlock" aria-hidden="true"></i></span>
                </div>
                  <input type="text" class="form-control" placeholder="password"  style="border-radius:  0px 50px 50px 0px;">
                </div>                  
                <a  class="mainfont a3" href="#"  style="float:right;font-size:12px;">
                    forgot password?
                </a>
              </b-col>
          </b-row> 
          <b-row>
              <b-col>
              </b-col>
          </b-row>         
          <b-row>              
            <b-col>
                <hr>
                  <div class="float-right">
                    <button class="btn btn-1 border" @click="showLoginSignupModal=false" style="color:var(--main-primary-color);border:2px solid black;margin-right:15px;">Cancel</button>
                    <button class="btn btn-1 btn-2 px-2">Login</button>
                  </div>
            </b-col>              
          </b-row>
      </b-container>
  </b-tab>
  <b-tab title="Signup" active>
      <b-container fluid style="margin-top: 50px;">
          <b-row>
              <b-col>
                <div class="input-group mb-3">
                <div class="input-group-prepend" >
                    <span class="input-group-text" style="border-radius: 50px 0px 0px 50px;">
                      <i class="fa fa-user" aria-hidden="true"></i>
                    </span>
                </div>
                  <input type="text" class="form-control" placeholder="email/mobile number" style="border-radius:  0px 50px 50px 0px;">
                </div>                  
              </b-col>
          </b-row>
          <b-row>
              <b-col>
                <div class="input-group mb-3">
                <div class="input-group-prepend" >
                    <span class="input-group-text" style="border-radius: 50px 0px 0px 50px;"><i class="fa fa-unlock" aria-hidden="true"></i></span>
                </div>
                  <input type="text" class="form-control" placeholder="password"  style="border-radius:  0px 50px 50px 0px;">
                </div>                  
              </b-col>
          </b-row> 
          <b-row>
              <b-col>
              </b-col>
          </b-row>         
          <b-row>              
            <b-col>
                <hr>
                  <div class="float-right">
                    <button class="btn btn-1 border" @click="showLoginSignupModal=false" style="color:var(--main-primary-color);border:2px solid black;margin-right:15px;">Cancel</button>
                    <button class="btn btn-1 btn-2 px-2">Signup</button>
                  </div>
            </b-col>              
          </b-row>
          <b-row>
            <b-col>
              <br>
              <p class="mainfont text-center" style="font-size:12px;">By signing up you agree to our
              <a href="#">"Terms of Policy</a>, <a href="">Privacy agreement"</a></p>
            </b-col>
          </b-row>
      </b-container>
  </b-tab>
</b-tabs>                    
                </b-col>
            </b-row>
        </b-container>
    </b-modal>     
</b-container>
</template>

<script>
    export default {
        name: 'LoginSignupModal',
        data: function() {
            return {
                showLoginSignupModal: false,

            }
        }
    };

</script>
<style>
    a {
        color: #68b8b6;
    }

    a:hover {
        color: #b8bbbb;
    }

    .input-box {
        border-radius: 20px;
    }

    input::placeholder {
        text-align: center;
    }

    input {
        text-align: center;

    }
    .btn-1 {
        border-radius: 20px;
        width: 95px;
        padding: 3px;
        margin: auto;
        background-color: #fff;
    }
    .btn-2 {
        background-color: var(--main-primary-color);
        color: #fff;
    }
    .modal-backdrop {
        background-color: var(--main-primary-color);
    }

    .modal-content {
        border-radius: 25px;
    }    
</style>
