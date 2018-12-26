<template>
  <div class="about">
      <VueLogoImage />
      <test msg="This is an test page"/>
      <about msg="This is an about page"/>
      <p>
        <button @click="pop">Click me!</button>
      </p>
      <div :class="{ show: isActive }" class="hide">ADDTOCART<br>ADDTOCART<br>ADDTOCART<br>ADDTOCART<br>ADDTOCART</div>
    
  </div>
</template>

<style>
.hide {
  display: none;
}
.show {
  display: block;
}
</style>


<script>
import VueLogoImage from '@/components/VueLogoImage.vue'
import test from '@/components/test.vue'
import about from '@/components/about.vue'


export default {
  name: 'home',
  data: function () {
    return {
      isActive: false,
    }
  },
  methods: {
    pop: function() {
      this.isActive = true
    }
  },
  components: {
    VueLogoImage,
    test,
    about
  }
}
</script>