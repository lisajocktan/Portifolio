<template>
<v-app>
    <Navpage />
<v-container class="content">
    <h4>ABOUT <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></h4>
    <h1 class="mt-5">LEARN MORE ABOUT ME</h1>
  <v-row>
    <v-col cols="4" class="bg"></v-col>
    <v-col cols="8">
          <h5 class="blue--text text--darken-4">Hello I'm Emil Jones</h5>
          <h1 class="white--text">UI/UX & Graphic Designer</h1>
          <p class="grey--text">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. <br />
            Adipisci explicabo, cupiditate necessitatibus iure hic omnis est ab
            <br />
            At nihil et temporibus ratione!
          </p>
      <v-row>
          <v-col cols="6">
        <v-list-item v-for="item in items" :key="item.text">
          <v-list-item-icon>
            <v-icon color="green darken-2">{{item.icon}}</v-icon>
          </v-list-item-icon >
          <v-list-item-content>
            <v-list-item-title class="white--text">{{item.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
          </v-col>
          <v-col cols="6">
            <v-list-item v-for="item in items" :key="item.text">
          <v-list-item-icon>
            <v-icon color="green darken-2">{{item.icon}}</v-icon>
          </v-list-item-icon >
          <v-list-item-content>
            <v-list-item-title class="white--text">{{item.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
          </v-col>
       </v-row>
       <p class="grey--text">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. <br />
            Adipisci explicabo, cupiditate necessitatibus iure hic omnis est ab
            <br />
            At nihil et temporibus ratione!
          </p>
    </v-col>
  </v-row>
 <v-row class="mt-5">
                <div class="card mt-5" v-for="list in lists" :key="list.text" >
                  <v-icon color="green" x-large class="ml-3">{{list.icon}}</v-icon>
                  <h1 class="white--text ml-3 mt-4">{{list.number}}</h1>
                  <p class="grey--text ml-3 mt-6"> {{list.text}} </p>
                </div>
 </v-row>
 <h4 class="mt-5">INTERESTS <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span></h4>
 <v-row class="mt-5">
      <v-col cols="3">
        <v-list-item v-for="like in likes" :key="like.text">
          <v-list-item-icon>
            <v-icon color="green darken-2">{{like.icon}}</v-icon>
          </v-list-item-icon >
          <v-list-item-content>
            <v-list-item-title class="white--text">{{like.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-col>
      <v-col cols="3">
        <v-list-item v-for="like in likes" :key="like.text">
          <v-list-item-icon>
            <v-icon color="green darken-2">{{like.icon}}</v-icon>
          </v-list-item-icon >
          <v-list-item-content>
            <v-list-item-title class="white--text">{{like.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-col>
<v-col cols="3">
        <v-list-item v-for="like in likes" :key="like.text">
          <v-list-item-icon>
            <v-icon color="green darken-2">{{like.icon}}</v-icon>
          </v-list-item-icon >
          <v-list-item-content>
            <v-list-item-title class="white--text">{{like.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-col>
      <v-col cols="3">
        <v-list-item v-for="like in likes" :key="like.text">
          <v-list-item-icon>
            <v-icon color="green darken-2">{{like.icon}}</v-icon>
          </v-list-item-icon >
          <v-list-item-content>
            <v-list-item-title class="white--text">{{like.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-col> </v-row>
</v-container>
</v-app>
</template>

<script>
import Navpage from '../components/Navpage'
export default {
  name: 'AboutView',

    components: {
      Navpage,
    },
     data: () => ({
      items: [
        { text: 'Birthday: 1 May 1995', icon: 'mdi-greater-than' },
        { text: 'Website: www.example.com', icon: 'mdi-greater-than' },
        { text: 'Phone: +255 752 186 174', icon: 'mdi-greater-than' },
        { text: 'City: New York, USA', icon: 'mdi-greater-than' },
      ],
      lists: [
        { text: 'Happy Clients', number:'232', icon: 'mdi-emoticon-happy-outline' },
        { text: 'Projects',number:'521', icon: 'mdi-projector-screen' },
        { text: 'Hour of Support',number:'1463', icon: 'mdi-timer' },
        { text: 'Award, USA',number:'24', icon: 'mdi-medal' },
      ],
       likes: [
        { text: 'Lorem Ipsum', icon: 'mdi-form-textbox' },
        { text: 'Magni Dolores', icon: 'mdi-forum' },
        { text: 'Midela Teren', icon: 'mdi-food-drumstick-outline' },
      ],
    }),
  }

</script>

<style scoped>
div[data-app='true'] {
  background: url('/public/6.png') no-repeat center center fixed ;
  background-size: cover;
}
span{
  border-bottom: 2px solid #18d26e;
  padding-bottom: 6px;
}
.content{
  width: 50%;
  color: white;
  background: rgba(0, 0, 0, 0.5); /* Black background with 0.5 opacity */
  margin-top: 20px;
  margin-bottom: 20px;
}
.bg{
  background: url('/public/1.png')no-repeat center center fixed ;
}
.card{
  margin-left: 100px;
}
</style>
