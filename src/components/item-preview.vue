<template>
  <li v-if="item">
      <custom-card>
      <template #header>
        <div class="prevImg">
          <img src="{{item.prevImg}}" alt="prevImg" />
          </div>        
      </template>
      <template #main>
        <p class="title">{{ item.title }} </p>
      </template>
      <template #footer>
        <p>{{ item.context }}</p>
      </template>
    </custom-card>

 </li>
</template>

<script>
  import customCard from './custom-card.vue';
export default {
  props: {
    item: Object,
  },


  computed:{
    getImage(){
      const src = this.item.prevImg
      return  `'${src}'`
    }

  },


  components:{
    customCard,
  }
};
</script>

<style></style>
