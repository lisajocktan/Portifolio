<template>
    <v-app-bar app color="#111111" dark flat class="px-8">
    <v-btn text>
      <h3>Emil Jones</h3>
    </v-btn>

    <v-spacer></v-spacer>
    <v-btn text v-for="link in links" :key="link.text" router :to="link.route">{{link.text}}</v-btn>
  </v-app-bar>
</template>

<script>
export default {
name: 'NavpagePage',
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