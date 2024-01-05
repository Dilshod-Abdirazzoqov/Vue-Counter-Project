<template>
    <div id="container">
      <h1>Counter: {{counter}}</h1>

      <div class="d-flex justify-content-between mx-3">
        <button type="button" class="btn btn-success" @click="inc">Add</button>
        <button type="button" class="btn btn-warning" @click="dec">Delete</button>
      </div>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        counter: 0
      }
    },
    methods: {
      inc () {
        this.counter +=1;
      },

      dec () {
        this.counter -=1;
      }
    }
  }
</script>



<style>
#container{
   width:20rem;
   margin:15rem auto;
   text-align:center;
}

#container h1{
  border: 1px solid #eee;
}
</style>
