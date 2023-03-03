<template>
    <button class="btn btn-primary" @click="filtered">Filter</button>
    <div class="container">
        <div v-for="product in products" :key="product.id">
        <div class="card" style="width: 12rem;">
            <img :src="product.imgURL" class="card-img-top" alt="...">
            <div class="card-body">
                <h5 class="card-title">{{ product.prodName }}</h5>
                <p class="card-text">{{product.prodDescription}}</p>
                <p class="card-text">R {{product.price}}</p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
            </div>
        </div>
    </div>
    </div>
    
</template>

<script>
export default {
    name: 'ProductsView',
    components: {

    },
    computed: {
        products() {
            return this.$store.state.products;
        },

        
    },

    mounted() {
            this.$store.dispatch("getProducts")
        }

}
</script>

<style scoped>
    .container{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        column-gap: .2rem;
        margin-top: 2rem;
    }
    .card{
        margin: 2rem;
        height: 450px;
    }
    /* img{
        
    } */
    @media screen and (max-width: 900px) {
        .container{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
    }
    }
    @media screen and (max-width: 600px) {
        .container{
        display: grid;
        grid-template-columns: 1fr 1fr;
    }
    }
    @media screen and (max-width: 400px) {
        .container{
        display: grid;
        grid-template-columns: 1fr;
    }
    }
</style>