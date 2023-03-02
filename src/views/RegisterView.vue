<template>
    <div>
       <h1>register</h1> 
    </div>
</template>

<script>
export default {
    name: 'RegisterView',
  components: {
   
  },
   computed: {
    products(){
    return this.$store.state.products;
  },

  mounted() {
    this.$store.dispatch("getProducts")
  }
    
  }
     
}

</script>

<style>

</style>