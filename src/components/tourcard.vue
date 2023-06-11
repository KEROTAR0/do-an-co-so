<template>
    <div class="container mt-5">
        <h1 class="text-center"> CÁC TOUR NỔI BẬT</h1>
        <div class="row justify-content-center">
            <div v-for="content in contents" :key="content.id" class="col-12 col-lg-4 col-md-6 mt-4" style="width: 24rem;">
                <div class="card">
                    <img v-bind:src="content.image" class="card-img-top" alt="...">
                    <div class="card-body text-center p-0 ps-3 pe-3">
                        <div class="title" style="height: 50px">
                            <a href="#" class="card-text m-0"> {{ content.title }}</a>
                        </div>
                        <span class="price"> {{ content.price }} VND </span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

 
<script>
import axios from 'axios'

export default {
    data() {
        return {
            contents: null
        }
    },
    mounted() {
        axios
            .get('http://localhost:3000/tour')
            .then((response) => (this.contents = response.data))
    }
}
</script>



<style scoped>
.card-img-top {
    width: 100%;
    height: 260px;
}

h1 {
    font-family: 'Roboto', sans-serif;
    font-weight: 700;
    color: #E86A33;

}

.price {
    color: #ED2B2A;
    font-size: large;
    font-weight: 700;
}

.title a{
    text-decoration: none;
    font-weight: 600;
    color: #2B7A0B;
}
</style>




