<template>
    <div v-for="product in products" :key="product.id">
        <div class="card" style="width: 18rem;">
            <img src="" class="card-img-top" alt="...">
            <div class="card-body">
                <h5 class="card-title">{{ product.prodName }}</h5>
                <p class="card-text">{{product.prodDescription}}</p>
                <p class="card-text">{{product.price}}</p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
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

        mounted() {
            this.$store.dispatch("getProducts")
        }
    }

}
</script>