<template>
  <v-app id="inspire">
    <v-navigation-drawer
      fixed
      v-model="drawer"
      app
    >
      <v-list dense>

        <v-list-tile @click="doM1">
          <v-list-tile-action>
            <v-icon>home</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Home</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>

        <v-list-tile @click="doM2">
          <v-list-tile-action>
            <v-icon>account_box</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Login</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>

        <v-list-tile @click="doM3">
          <v-list-tile-action>
            <v-icon>description</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Post Product</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>

        <v-list-tile @click="doM4">
          <v-list-tile-action>
            <v-icon>spa</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Product List</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>

        <v-list-tile @click="doM5">
          <v-list-tile-action>
            <v-icon>receipt</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Edit Product</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>

        <v-list-tile @click="doM6">
          <v-list-tile-action>
            <v-icon>contact_mail</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Contact</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>


      </v-list>
    </v-navigation-drawer>
    <v-toolbar color="indigo" dark fixed app>
      <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
      <v-toolbar-title>OTOP Market</v-toolbar-title>
    </v-toolbar>
    <v-content>
      <nuxt />
    </v-content>
    <v-footer color="indigo" app>
      <span class="white--text">&copy; 2017</span>
    </v-footer>
  </v-app>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>

<script>
export default {
  methods: {
    doM1(){
      this.$router.push('/')
    },
    doM2(){
      this.$router.push('')
    },
    doM3(){
      this.$router.push('/product-post')
    },
    doM4(){
      this.$router.push('/product-list')
    },
    doM5(){
      this.$router.push('/product-list-for-edit')
    },
    doM6(){

    },
    drawer(){
      
    }

  }
}
</script>
