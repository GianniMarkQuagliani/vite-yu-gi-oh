<script>
import { store } from '../data/store';
import CharacterCard from './partials/CharacterCard.vue';
export default {
  nome: 'CardsContainer',
  components:{
    CharacterCard
  },
  data (){
    return{
      store
    }
  },
  mounted(){
    console.log(store.charctersList);
  }
}
</script>


<template>
  <div class="container my-5">
    <div class="row">
      <CharacterCard
      v-for="card in store.charctersList" 
      :key="card.id" 
      :image="card.card_images[0].image_url" 
      :name="card.name" 
      :frameType="card.frame" />
    </div>
  </div>
</template>


<style lang="scss" scoped>

</style>