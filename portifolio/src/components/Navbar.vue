<template v-slot:extension>
<v-tabs center-active background-color="#1B1A1A" dark max-width="auto">
    <v-tabs-slider color="#18d26e"></v-tabs-slider>
    <v-tab class="font-weight-light"  v-for="link in links" :key="link.text" router :to="link.route">{{link.text}}</v-tab>
  
</v-tabs>

</template>

<script>
export default {
    name:'NavbarPage',
    data() {
    return {
        
        links: [
        {text: 'Home', route: '/' },
        {text: 'About', route: '/about' },
        {text: 'Resume', route: '/resume' },
        {text: 'services', route: '/services' },
        {text: 'Portifolio', route: '/portifolio' },
        {text: 'Contact', route: '/contact' },
      ]
    }
  }

}
</script>

<style>

</style>