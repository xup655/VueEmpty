<template>
  <div class="home">
      <VueLogoImage />
    <HelloWorld msg="Welcome to Empty Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import VueLogoImage from '@/components/VueLogoImage.vue'
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    VueLogoImage,
    HelloWorld
  }
}
</script>
