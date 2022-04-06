<template>
<app-header  class="main-layout"/>
<hero  class="main-layout"/>
<item-list class="main-layout" />
<productive class="main-layout" />
<reviews class="main-layout" />
<acess class="main-layout" />
<app-footer class="main-layout" />

</template>

 

<script >
import appHeader from '../src/components/app-header.vue'
import appFooter from '../src/components/app-footer.vue'
import hero from '../src/components/hero.vue'
import itemList from '../src/components/item-list.vue'
import productive from '../src/components/productive.vue'
import reviews from '../src/components/reviews.vue'
import acess from '../src/components/acess.vue'
export default {
  
  
  
  
  

  components:{
    appHeader,
    hero,
    itemList,
    productive,
    reviews,
    acess,
    appFooter
  }

}



</script>

<style>

</style>
