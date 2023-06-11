<template>
    <nav class="navbar navbar-expand-lg  border-bottom border-danger border-opacity-50 fixed-top">
        <div class="container-fluid">
            <a class="navbar-logo col-5 text-center" href="/">
                <img src="../assets/images/iconHeader.png" alt="Logo" width="90px">
                <!-- <router-link to="/"> home </router-link> -->

            </a>

            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link active text-uppercase fw-bold" aria-current="" href="/intro">Giới thiệu</a>
                    </li>
                    
                    <li class="nav-item-dropdown ">
                        <a class="nav-link dropdown text-uppercase  fw-bold" href="/Tour" > Tour </a>
                        <ul class="dropdown-content p-0">
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Tour nội thành Đà Lạt</a></li>
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Tour ngoại thành Đà Lạt</a></li>
                        </ul>
                    </li>

                    <li class="nav-item-dropdown ">
                        <a class="nav-link dropdown text-uppercase fw-bold" href="#" > Khách sạn </a>
                        <ul class="dropdown-content p-0">
                            <li><a class="dropdown-item p-1 pe-5 fw-semibold" href="#">Biệt thự Đà Lạt</a></li>
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Khách sạn 5 sao</a></li>
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Khách sạn 4 sao</a></li>
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Khách sạn 3 sao</a></li>
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Khách sạn 2 sao</a></li>
                            <li><a class="dropdown-item p-1 fw-semibold" href="#">Khách sạn 1 sao</a></li>
                        </ul>
                    </li>

                    <li class="nav-item ">
                        <a class="nav-link active text-uppercase fw-bold" aria-current="page" href="#">Dịch vụ</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link active text-uppercase fw-bold" aria-current="page" href="/CamNang">Cẩm nang du lịch</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link active text-uppercase fw-bold" aria-current="page" href="#">Tin tức</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link active text-uppercase fw-bold" aria-current="page" href="#">Liên hệ</a>
                    </li>
                </ul>
            </div>
        </div>

       
    </nav> 
    
</template>




<script>
export default {
}
</script>

<style scoped>
nav{
    background-color: #EEEEEE;
}


a {
    text-decoration: none;
    /* color: #2D2727; */
    font-size: 18px;
    color: black;

}

.nav-item-dropdown{
    position: relative;
    display: inline-block;
    
}


/* submenu */
.dropdown-content{
    list-style: none;
    display: none;
    position: absolute;
    z-index: 1;
    background-color:#E86A33;

    
}



.nav-item-dropdown:hover .dropdown-content{
    display: block;
    
}

.nav-item-dropdown:hover>a{
    background-color: #E86A33;
    color: #EEEEEE;
}

.nav-item a:hover{
    color: #EEEEEE;
}



.nav-item:hover{
    background-color: #E86A33;
    color: #EEEEEE;
}

.nav-item-dropdown ul li:hover{
    color: #EEEEEE;
}


</style>