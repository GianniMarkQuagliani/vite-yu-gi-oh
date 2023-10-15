<script>

import axios from 'axios';
import { store } from './data/store';
import Header from './components/Header.vue';
import CardsContainer from './components/CardsContainer.vue';
import Results from './components/partials/Results.vue';
import SearchBar from './components/partials/SearchBar.vue';

export default {
    name: 'App',
    components: {
        Header,
        CardsContainer,
        Results,
        SearchBar
    },
    data(){
        return{
            store
        }
    },
    methods :{
        // chiamata API
        getApi(){
            axios.get(store.apiUrl, {
                params:{
                  name: store.nameToSearch,
                  archetype: store.archetypeToSearch
                  
                }
            })
            .then( res =>{
                store.charctersList = res.data.data;
                console.log(store.charctersList[0].card_images[0].image_url);
            })
            .catch(err => {
                console.log(err);
            })
        }
    },
    mounted(){
        this.getApi();
    }
}
</script>


<template>
  <Header titleStr="Vite Yu-Gi-Oh" />
  <SearchBar @startSearch="getApi" />
  <Results />
  <CardsContainer />
  
</template>


<style lang="scss" scoped>
@use './scss/main.scss';
</style>