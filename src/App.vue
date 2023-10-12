<script>

import axios from 'axios';
import { store } from './data/store';
import Header from './components/Header.vue';
import CardsContainer from './components/CardsContainer.vue';
import Resuts from './components/partials/Resuts.vue';

export default {
    nome: 'App',
    components: {
        Header,
        CardsContainer,
        Resuts
    }
}
</script>


<template>
  <Header titleStr="Vite Yu-Gi-Oh" />
  <Resuts />
  <CardsContainer />
  
</template>


<style lang="scss" scoped>
@use './scss/main.scss';
</style>