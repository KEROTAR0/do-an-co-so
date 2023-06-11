<template>
    <div class="position-relative">
            <img src="../assets/images/bgslide.jpg" class="d-block w-100 bg-img" alt="backgroundslider">
            <div class="carousel-caption top-0 mt-2">
                <div id="coursel-slide" class="carousel slide w-100" data-bs-ride="carousel">
                    <!-- ba gach -->
                    <div class="carousel-indicators">
                        <button type="button" data-bs-target="#coursel-slide" data-bs-slide-to="0" class="active"
                            aria-current="true" aria-label="Slide 1"></button>
                        <button type="button" data-bs-target="#coursel-slide" data-bs-slide-to="1"
                            aria-label="Slide 2"></button>
                        <button type="button" data-bs-target="#coursel-slide" data-bs-slide-to="2"
                            aria-label="Slide 3"></button>
                        <button type="button" data-bs-target="#coursel-slide" data-bs-slide-to="3"
                            aria-label="Slide 3"></button>
                        <button type="button" data-bs-target="#coursel-slide" data-bs-slide-to="4"
                            aria-label="Slide 3"></button>
                    </div>

                    <div class="carousel-inner">
                        <div class="carousel-item active c-item" data-bs-interval="2000">
                            <img src="../assets/images/slide1.jpg" class="d-block w-100 c-img" alt="slide1">
                        </div>
                        <div class="carousel-item c-item" data-bs-interval="2000">
                            <img src="../assets/images/slide2.jpg" class="d-block w-100 c-img" alt="slide2">
                        </div>
                        <div class="carousel-item c-item" data-bs-interval="2000">
                            <img src="../assets/images/slide3.jpg" class="d-block w-100 c-img" alt="slide3">
                        </div>
                        <div class="carousel-item c-item" data-bs-interval="2000">
                            <img src="../assets/images/slide4.jpg" class="d-block w-100 c-img" alt="slide4">
                        </div>
                        <div class="carousel-item c-item">
                            <img src="../assets/images/slide5.jpg" class="d-block w-100 c-img" alt="slide15">
                        </div>
                    </div>

                    <button class="carousel-control-prev" type="button" data-bs-target="#coursel-slide"
                        data-bs-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Previous</span>
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#coursel-slide"
                        data-bs-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Next</span>
                    </button>
                </div>

            </div>
        </div>
        
</template>



<script>
export default {
    
}
</script>



<style>
.position-relative{
    margin-top: 97px;
}


.bg-img {
    height: 580px;
    width: 100%;
    object-fit: cover;
    opacity: 50%;
}

.c-item {
    height: 530px;
}

.c-img {
    height: 100%;
    object-fit: cover;

}</style>