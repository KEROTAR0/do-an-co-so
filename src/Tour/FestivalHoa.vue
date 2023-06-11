<template>
  <compheader/>
  <compslider/>

    <div class="container ps-5 pe-5 mt-4">
        <div class="content">
            <h3>LỊCH KHỞI HÀNH TOUR FESTIVAL HOA ĐÀ LẠT 2023</h3>
            
            <div class="d-flex">
                <div class="p-2 flex-fill">                    
                    <img src="../assets/images/Tour/tour-du-lich-festival-hoa-da-lat.jpg" class="card-img-top" alt="...">
                </div>
                <div class="p-2 flex-fill">
                    <div class="d-flex flex-column mb-3">
                        <div class="p-2">Mã Tour: ZT0033</div>
                        <div class="p-2">Thời gian: 3 ngày 3 đêm</div>
                        <div class="p-2">Loại xe: Giường nằm/ ghế ngã</div>
                        <div class="p-2">Tour đã bao gồm:</div>
                        <div class="p-2">+ Khách sạn 2 sao</div>
                        <div class="p-2">+ Vé tham quan </div>
                        <div class="p-2">+ Phương tiện</div>
                        <div class="p-2">+ Ăn uống</div>
                        <div class="p-2">+ Vé Buffet rau</div>

                    </div>
                </div>
                <div class="p-2 flex-fill">
                    
                    Giá Tour: <b id="price-display">1.890.000đ</b>
                </div>
            </div>
        </div>
    </div>

  <compfooter/>
</template>
  




<script>



  import compheader from '../components/compheader.vue';
  import compslider from '../components/compslider.vue';
  import compfooter from '../components/compfooter.vue';

export default {
  components: {
    compheader,
    compslider,
    compfooter

  }
}

</script>

<style scoped>
img{
    size: 50%;
}
b{
    font-size: 30px;
    color: #ff3131;
}
h3{
  font-family: 'Times New Roman', Times, serif;
  color: #E86A33;
}
h4{
  font-family: 'Times New Roman', Times, serif;
  color: #ff3131;
}
</style>
  