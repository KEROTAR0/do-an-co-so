<template> 
      <div class="container mt-5">
        <h1 class="text-center"> TIN TỨC - BÀI VIẾT MỚI </h1>
        <div class="row justify-content-center">
            <div v-for="content in contents" :key="content.id" class="col-12 col-lg-4 col-md-6 mt-4" style="width: 20rem;">
                <div class="card">
                    <img v-bind:src="content.image" class="card-img-top" alt="...">
                    <div class="card-body  p-0 ps-2 pe-2">
                        <div class="title" style="height: 50px">
                            <a href="#" class="card-text m-0 text-uppercase"> {{ content.title }}</a>
                        </div>
                        <p> {{ content.detail.intro}}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>



<script> 
import axios from 'axios';

    export default{
        data(){
            return{
                contents:null
            }
        },
        mounted(){
            axios
                .get('http://localhost:3000/neus')
                .then((response) => (this.contents = response.data))
            
        }

    } 


</script>




<style scoped>
.card-img-top {
    width: 100%;
    height: 230px;
}

h1 {
    font-family: 'Roboto', sans-serif;
    font-weight: 700;
    color: #E86A33;

}

.title a{
    text-decoration: none;
    font-weight: 600;
    color: #1587bb;
}

/* css cắt đoạn */
p {
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
  overflow: hidden;
}


</style>