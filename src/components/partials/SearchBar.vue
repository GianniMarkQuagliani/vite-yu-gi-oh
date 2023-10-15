<script>
export default {
    name: 'SearchBar'
}
</script>


<template>
  <div class="container">
    <div class="row justify-content-center">
        <div class="col-auto">
            <input type="text" class="form-control" placeholder="Search">
        </div>
        <div class="col-auto">
            <select name="form-control" aria-label="Default select example">
                <option selected>Select Status</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
            </select>
        </div>
        <div class="col-auto">
            <button @click="$emit('startSearch')" class="btn btn-info">Search</button>
        </div>
        <div class="col-auto">
            <button class="btn btn-warning">Reset</button>
        </div>
    </div>
  </div>
</template>



<style lang="scss" scoped>

</style>