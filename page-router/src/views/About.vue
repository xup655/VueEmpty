<template>
  <div class="about">
      <img alt="Vue logo" src="../assets/logo.png">
      <test msg="This is an test page"/>
      <about msg="This is an about page"/>
    
  </div>
</template>

<script>
import test from '@/components/test.vue'
import about from '@/components/about.vue'


export default {
  name: 'home',
  components: {
    test,
    about
  }
}
</script>