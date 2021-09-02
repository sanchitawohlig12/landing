<template>
  <div>
    <h1>Contact Us</h1>
    <h1></h1>
    <p>
      Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas
      accumsan lacus vel facilisis.
    </p>
    
    <v-row class="align-center">
      <v-col cols="12" sm="8">
        <p v-if="error.length">
      <marquee width="40%" >
        Missed Something
      </marquee>
      <ul class="u1">
        <li v-for="e in error" v-bind:key="e.id" class="ListErrors">{{e}}
          
        </li>
      </ul>

    </p>
        <form @submit="Login">
          <v-sheet class="mx-auto pa-4" elevation="8" max-width="800">
            <v-row>
              <v-col cols="12" sm="12">
                <v-row>
                  <v-col cols="12" sm="6">
                    <v-text-field
                      v-model="name"
                      label="Name"
                      outlined
                      clearable
                      color="pink"
                      
                    ></v-text-field>
                  </v-col>
                  <v-col cols="12" sm="6">
                    <v-text-field
                    type="email"
                      v-model="email"
                      label="Email"
                      outlined
                      clearable
                      color="pink"
                      required
                      
                    ></v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="12" sm="6">
                    <v-text-field
                      v-model="subject"
                      label="Subject"
                      outlined
                      clearable
                      color="pink"
                      
                    ></v-text-field>
                  </v-col>
                  <v-col cols="12" sm="6">
                    <v-text-field
                    type="number"
                      v-model="phone"
                      label="Phone Number"
                      outlined
                      clearable
                      color="pink"
                      
                    ></v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="12" sm="12">
                    <v-textarea
                      v-model="message"
                      outlined
                      name="input-7-4"
                      label="Solo textarea"
                      color="pink"
                      
                    ></v-textarea>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="12" sm="12">
                    <v-btn
                      type="submit"
                      value="Submit"
                      depressed
                      color="pink"
                      rounded
                      class="white--text"
                      large
                    >
                      Send Message
                    </v-btn>
                  </v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-sheet>
        </form>
      </v-col>
      <v-col cols="12" sm="4">
        <v-sheet class="mx-auto" elevation="8" max-width="500" max-height="300">
          <v-list two-line>
            <v-list-item>
              <v-list-item-icon>
                <v-icon color="pink"> mdi-map-marker </v-icon>
              </v-list-item-icon>

              <v-list-item-content>
                <v-list-item-title class="grey--text text--darken-3"
                  ><b>Address: </b></v-list-item-title
                >
                <v-list-item-subtitle
                  >1828 Johns Drive Glenview, IL 60025</v-list-item-subtitle
                >
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-icon>
                <v-icon color="pink"> mdi-email </v-icon>
              </v-list-item-icon>

              <v-list-item-content>
                <v-list-item-title class="grey--text text--darken-3"
                  ><b>Email: </b></v-list-item-title
                >
                <v-list-item-subtitle>support@ganial.com</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-icon>
                <v-icon color="pink"> mdi-phone </v-icon>
              </v-list-item-icon>

              <v-list-item-content>
                <v-list-item-title class="grey--text text--darken-3"
                  ><b>Phone: </b></v-list-item-title
                >
                <v-list-item-subtitle>(224) 228-8475</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-list-item>
              <v-list-item-icon>
                <v-icon color="pink"> mdi-web </v-icon>
              </v-list-item-icon>

              <v-list-item-content>
                <v-list-item-title class="grey--text text--darken-3"
                  ><b>Website: </b></v-list-item-title
                >
                <v-list-item-subtitle>www.ganial.com</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-sheet>
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {
  name: 'contact',

  data() {
    return {
      error: [],
      name: null,
      email: null,
      message: null,
      subject: null,
      phone: null,
    }
  },
  methods: {
    Login(e) {
      if (
        this.name &&
        this.email &&
        this.message &&
        this.phone &&
        this.subject
      ) {
        console.log('successfully done')
        alert('Thanks for contacting us...!')
      }
      this.error = []
      if (!this.name) {
        this.error.push('Please Enter Name..!')
      }
      if (!this.email) {
        this.error.push('Please Enter Email')
      }
      if (!this.phone) {
        this.error.push('Please Enter Phone Number ')
      }
      if (!this.subject) {
        this.error.push('Please Enter subject')
      }
      if (!this.message) {
        this.error.push('Please Enter a Message for us..!')
      }
      console.warn('Error:' + this.error)
      e.preventDefault()
      this.name = ''
      this.email = ''
      this.message = ''
      this.subject = ''
      this.phone = ''
    },
  },
}
</script>
<style scoped>
h1 {
  text-align: center;
}
p {
  text-align: center;
}
.u1 {
  color: rgb(190, 21, 49);
  list-style-type: none;
}
</style>