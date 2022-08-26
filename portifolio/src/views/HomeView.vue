<template>
<v-app class="app">
<v-container fluid class="d-sm-flex">
 <v-row>
  <v-col cols="6" class="grid1">
    <h1 class="white--text top">Emily Jones</h1><br>
    <h3 class="font-weight-light white--text">I am a passionate <span>Graphic Designer</span> from New York</h3>
     <br>
     <p><Navbar /></p><br>
     <p><v-row justify="left">
    <v-icon medium color="white" class="fa"> mdi-twitter</v-icon>
    <v-icon medium color="white" class="fa">mdi-facebook</v-icon>
    <v-icon medium color="white" class="fa"> mdi-instagram</v-icon>
    <v-icon medium color="white" class="fa"> mdi-linkedin</v-icon>
    
    </v-row>
    </p>
  </v-col>
 </v-row>
</v-container>



  </v-app>
</template>

<script>
  import Navbar from '../components/Navbar'

  export default {
    name: 'HomePage',

    components: {
      Navbar,
    },
  }
</script>
<style scoped>
.top{
  margin-top:180px; 
  
}
.fa {
  padding: 20px;
  margin: 5px 2px;
  border-radius: 50%;
  background-color: rgb(5, 5, 5);
}
.fa:hover {
    opacity: 0.7;
    color: greenyellow;
}
div[data-app='true'] {
  background: url('/public/6.png') no-repeat center center fixed ;
  background-size: cover;
}
.grid1{
  margin-left: 180px;
  margin-top:140px; 
}
h1{
  font-size: 48px;
  margin: 0;
  padding: 0;
  line-height: 1;
  font-weight: 700;
  font-family: "Poppins", sans-serif;
}
span{
  border-bottom: 2px solid #18d26e;
  padding-bottom: 6px;
}

</style>