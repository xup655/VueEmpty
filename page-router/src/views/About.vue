<template>
  <div class="about">
      <VueLogoImage />
      <test msg="This is an test page"/>
      <about msg="This is an about page"/>
    
  </div>
</template>

<script>
import VueLogoImage from '@/components/VueLogoImage.vue'
import test from '@/components/test.vue'
import about from '@/components/about.vue'


export default {
  name: 'home',
  components: {
    VueLogoImage,
    test,
    about
  }
}
</script>