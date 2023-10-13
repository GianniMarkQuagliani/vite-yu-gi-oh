<script>
export default {
  nome: 'CharacterCard',
  props:{
    image: String,
    name: String
  }
}
</script>


<template>
      
  <div class="card-deck">
    <div class="card">
      <img class="card-img-top" src="https://images.ygoprodeck.com/images/cards/73262676.jpg" alt="Card image cap">
      <div class="card-body">
        <p>bla bla</p>
          <p>bla bla</p>
          <p>bla bla</p>
          <p>bla bla</p>
      </div>
  </div>
  </div>
      
</template>


<style lang="scss" scoped>
.card{
  margin-bottom: 50px;
}

</style>