<template>
  <v-app>
    <v-content>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center">
          <v-col cols="12" sm="8" md="8"> 
            <v-card class="elevation-12">
              <v-window v-model="step">
                  <v-window-item :value="1">
                     <v-row>
                      <v-col cols="12" md="8">
                        <v-card-text class="12">
                          <h1 class="text-center display-2 success--text ">Sign in to NOTTECH </h1>
                          <div class="text-center mt-4">
                            <v-btn class="mx-2" fab color="primary" outlined>
                              <v-icon>fab fa-facebook-f</v-icon>
                            </v-btn>
                            <v-btn class="mx-2" fab color="red" outlined>
                              <v-icon>fab fa-google-plus-g</v-icon>
                            </v-btn>
                            <v-btn class="mx-2" fab color="red" outlined>
                              <v-icon>fab fa-instagram</v-icon>
                            </v-btn>
                            <v-btn class="mx-2" fab color="primary" outlined>
                              <v-icon>fab fa-linkedin-in</v-icon>
                            </v-btn>
                          </div>
                          <h4 class="text-center mt-8">You have email? Login</h4>
                          <v-form>
                           <v-text-field
                            label="Email"
                            name="email"
                            type="emal"
                            prepend-icon="mdi-email"
                          />
                          <v-text-field
                          id="password"
                          label="Password"
                          name="password"
                          type="password"
                          prepend-icon="mdi-lock"
                          />
                          </v-form>
                          <h4 class="text-center mt-3">Forgot your password?</h4>
                          <div class="text-center mt-3">
                          <v-btn rounded color="primary">Login</v-btn>
                        </div>
                        </v-card-text>
                      </v-col>
                       <v-col cols="12" md="4" class="orange accent-3">
                         <v-card-text class="white--text mt-12">
                           <h1 class="text-center display-1">Welcome NOTTECH !</h1>
                           <h5 class="text-center">Enter your personal details, happy code</h5>
                         </v-card-text>
                         <div class="text-center">
                           <v-btn rounded outlined="" dark @click="step++">sign up</v-btn>
                         </div>
                       </v-col>
                    </v-row>
                  </v-window-item>
                  <v-window-item :value="2">
                   <v-row class="fill-height">
                     <v-col cols="12" md="4" class="primary accet-3">
                       <v-card-text class="white--text mt-12">
                         <h1 class="text-center display-1">Welcome Back!</h1>
                         <h5 class="text-center">To keep intouch with us please login</h5>
                          <div class="text-center">
                            <v-btn rounded outlined primary @click="step--">Login</v-btn>
                       </div>
                       </v-card-text>
                     </v-col>
                     <v-col cols="12" md="8">
                       <v-card-text class="mt-12">
                         <h1 class="text-center display-2 primary--text text--accent-3">Create Account</h1>
                         <div class="text-center mt-4">
                           <v-btn class="mx-2" fab color="primary" outlined>
                             <v-icon>fab fa-facebook-f</v-icon>
                           </v-btn>
                            <v-btn class="mx-2" fab color="red" outlined>
                              <v-icon>fab fa-google-plus-g</v-icon>
                            </v-btn>
                            <v-btn class="mx-2" fab color="red" outlined>
                              <v-icon>fab fa-instagram</v-icon>
                            </v-btn>
                            <v-btn class="mx-2" fab color="blue" outlined>
                              <v-icon>fab fa-linkedin-in</v-icon>
                            </v-btn>
                         </div>
                         <h4 class="text-center mt-4">Please Create your Account</h4>
                         <v-form>
                           <v-text-field
                           label="name"
                           name="name"
                           prepend-icon="person"
                           type="text"

                           />
                           <v-text-field
                           label="Email"
                            name="email"
                            type="emal"
                            prepend-icon="mdi-email"
                           />
                          <v-text-field
                          id="password"
                          label="Password"
                          name="password"
                          type="password"
                          prepend-icon="mdi-lock"
                          />
                         </v-form>
                         <div class="text-center mt-5">
                         <v-btn rounded color="primary accet-3">sign up</v-btn>
                       </div>
                       </v-card-text>
                       
                     </v-col>
                   </v-row>
                  </v-window-item>
              </v-window>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data:()=>({
    step:1
  }),
  props:{
    source: String  
  }
}
</script>