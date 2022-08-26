<template>
<v-app>
    <Navpage />

</v-app>
</template>

<script>
import Navpage from '../components/Navpage'
export default {
  name: 'ResumePage',

    components: {
      Navpage,
    },
}
</script>

<style scoped>
div[data-app='true'] {
  background: url('/public/6.png') no-repeat center center fixed ;
  background-size: cover;
}

</style>
