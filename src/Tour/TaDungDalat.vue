<template>
  <compheader/>
  <compslider/>

    <div class="container ps-5 pe-5 mt-4">
      <div class="content">
        <h3>LỊCH KHỞI HÀNH TOUR FESTIVAL HOA ĐÀ LẠT 2023</h3>
            
        <div>
          <div >                    
            <img src="../assets/images/Tour/tour-ta-dung-da-lat.jpg" class="card-img-top" alt="...">
        </div>          
        <div class="d-flex justify-content-between">
          <div class="d-flex flex-column mb-3">
            <div class="p-2">Mã Tour: ZT0179</div>
            <div class="p-2">Thời gian: 3 ngày 2 đêm</div>
            <div class="p-2">Loại xe: Ôtô</div> 
          </div>
          <div >            
              <div class="d-flex flex-column mb-3">
                <div class="p-2">Chọn loại khách sạn: </div>
                <div class="p-2">
                  <input type="radio" id="hotel1" value="hotel1" v-model="selectedHotel">
                  <label for="hotel1">Khách sạn 2 sao</label>
                </div>
                <div class="p-2">
                  <input type="radio" id="hotel2" value="hotel2" v-model="selectedHotel">
                  <label for="hotel2">Khách sạn 3 sao</label></div>
              </div>        
          </div>
          <div class="d-flex flex-column mb-3">
            <div class="p-2">Tour đã bao gồm:</div>
            <div class="p-2">+ Khách sạn</div>
            <div class="p-2">+ Vé tham quan </div>
            <div class="p-2">+ Phương tiện</div>
            <div class="p-2">+ Ăn uống</div>
          </div>

        </div>

        <br>
        <div class="btn-toolbar mb-3" role="toolbar" aria-label="Toolbar with button groups">
          <div class="input-group">
            <div>
                <div class="price-display">
                  <p>Giá: </p>
                  <div v-if="selectedHotel === 'hotel1'">
                    <p>1.990.000đ</p>
                  </div>
                  <div v-if="selectedHotel === 'hotel2'">
                    <p>2.690.000đ</p>
                  </div>
                </div> 
            </div>
            
          </div>
          <div class="btn-group me-2" role="group" aria-label="First group">
            <button id="fontw" type="button" class="btn btn-outline-danger">Đặt Tour</button>
          </div>          
        </div>
        <br>
        <h3>Lịch trình chi tiết</h3>

        <div class="row">
          <div class="col-4">
            <div id="list-example" class="list-group stickyy">
              <a class="list-group-item list-group-item-action" href="#list-item-1">Ngày 1</a>
              <a class="list-group-item list-group-item-action" href="#list-item-2">Ngày 2</a>
              <a class="list-group-item list-group-item-action" href="#list-item-3">Ngày 3</a>
            </div>
          </div>
          <div class="col-8">
            <div data-bs-spy="scroll" data-bs-target="#list-example" data-bs-smooth-scroll="true" class="scrollspy-example" tabindex="0">
              <h5 id="list-item-1">Ngày 1</h5>
              <h5>TP.HCM – BẢO LỘC - DAK NÔNG (Ăn sáng/trưa/tối)</h5>
              <p><b>04h30:</b> Xe và HDV đón quý khách tại điểm hẹn, khởi hành tour Tà Đùng 3 ngày 2 đêm. khởi hành theo quốc lộ 20 đến Bảo Lộc, theo quốc lộ 28 qua các địa danh nổi tiếng và quang cảnh núi rừng hùng vĩ hai bên đường.</p>
              <p><b>07h30:</b> Đoàn đến Bảo Lộc, sau đó vào nhà hàng dùng điểm tâm sáng tại nhà hàng.</p>
              <p><b>09h30:</b> Đến Khu Bảo Tồn Thiên Nhiên Tà Đùng, qua con đường đèo dài, khung cảnh núi rừng hoang vu hiện ra với những đồi café, tiêu bạt ngàn phủ xanh núi đồi Tây Nguyên dọc 2 bên đường mang đến cho Quý khách trải nghiệm tuyệt vời.</p>
              <p>Đến Khu Bảo Tồn Thiên Nhiên Tà Đùng, qua con đường đèo dài, khung cảnh núi rừng hoang vu hiện ra với những đồi café, tiêu bạt ngàn phủ xanh núi đồi Tây Nguyên dọc 2 bên đường mang đến cho Quý khách trải nghiệm tuyệt vời.</p>
              <p><b>10h00:</b> Quý khách dừng chân tại Tà Đùng top view home stay hay còn gọi là nhà “Chú Đông”. Được xây dựng trên đồi cao thưởng thức cafe, trà hay các món kem mát lạnh tại đây (chi phí nước tự túc). Và không quên selfie những bức ảnh sống ảo, ngắm nhìn toàn cảnh hồ Tà Đùng với các hòn đảo nhấp nhô trên mặt hồ từ trên cao.</p>
              <p><b>12h00:</b> Quý khách dùng buổi trưa tại Tà Đùng, sau đó khởi hành đi Đà Lạt.</p>
              <p><b>17h00:</b> Đến với Đà Lạt, đoàn nhận phòng nghỉ ngơi tại khách sạn.</p>
              <p><b>18h00:</b> Xe đưa quý khách dùng cơm chiều tại nhà hàng.</p>
              <p><b>Tối:</b> Quý khách tự do dạo phố khám phá Đà Lạt về đêm hay tự do thưởng thức những món ăn đặc sản của ẩm thực Đà Lạt về đêm.</p>
              
              <h5 id="list-item-2">Ngày 2</h5>
              <h5>ĐỒI CHÈ CẦU ĐẤT – QUE GARDEN – ĐÀ LẠT VIEW (Ăn sáng/trưa/tối)</h5>
              <p><b>07h00:</b> Quý khách dùng điểm tâm sang tại nhà hàng, sau đó khởi hành khám phá các điểm mới trong tour Đà Lạt.</p>
              <p><b>08h00:</b> Quý Khách khởi hành tham quan các điểm.</p>
              <div class="d-flex flex-column mb-3">
                <div class="p-2">+ Đồi Chè Cầu Đất với những hàng chè hiện ra trong khung cảnh thiên nhiên hài hòa giữa màu xanh dương của đám mây kết hợp với hình ảnh núi đồi rợp lên một màu xanh lá cây trải dài từ dãy này qua dãy khác, cùng với những chú chim bay lượn trên cao tạo nên một bức tranh phong cảnh đẹp tuyệt vời.</div>
                <div class="p-2">+ Vườn hoa Cẩm Tú Cầu Đà Lạt, tại nới đây hoa Cẩm Tú cầu được trồng thành những cánh đồng bát ngát với nhiều màu sắc khác nhau, Quý khách được tự do sáng tại những kiểu ảnh đẹp lung linh.</div>
                <div class="p-2">+ Chùa Linh Phước – ngôi chùa đạt nhiều kỷ lục nhất Việt Nam. Với nhiều công trình kiến trúc kỳ vỹ được làm từ hơn 5.000 mảnh ve chai. Tượng Phật Bà Quan Âm được kết bằng hàng ngàn đóa hoa bất tử.</div>
              </div>
              <p><b>12h00:</b> Xe đưa đoàn đi ăn trưa tại nhà hàng. Sau khi dùng buổi trưa xe đưa đoàn về khách sạn nghĩ ngơi.</p>
              <p><b>14h30:</b> Khởi hành tham quan:</p>
              <div class="d-flex flex-column mb-3">
                <div class="p-2">+ QUE Garden tự hào là khu vườn bonsai lá kim lớn nhất Việt Nam. Những chậu cây bonsai vừa to vừa đẹp, được chăm sóc và uốn nắn kỹ lưỡng vô cùng đẹp mắt, và bạn khó có thể tìm thấy nhiều cây Bonsai đẹp như thế tại Việt Nam. Đặc biệt là hồ cá Koi theo tiêu chuẩn Nhật Bản, cùng với nhiều loài hoa hút hồn du khách đến đây.</div>
                <div class="p-2">+ Đà Lạt View Những tiểu cảnh được dựng lên ở nơi đây, chẳng khác chi những khung cảnh mà bạn đã từng bắt gặp trong những thước phim Hồng Kông xưa. Với gam đỏ chủ đạo, tất cả như nổi bật lên giữa không gian xanh ngát xanh của núi đồi. Tại đây quý khách được thỏa sức sáng tại ra những “pô” hình đẹp, độc với những cảnh đẹp Đà Lạt nổi tiếng như Cổng Trời, Cầu Tình Yêu…</div>
              </div>
              <p><b>17h30:</b> Quý khách dùng buổi tối, xe đưa quý khách về khách sạn.</p>
              <p><b>Tối:</b> Tự do khám phá Đà Lạt về đêm, thưởng thức những đặc sản tại chợ đêm Âm Phủ.  </p>

              <h5 id="list-item-3">Ngày 3</h5>
              <h5>THÁC VOI – CHÙA LINH ẨN – TP. HỒ CHÍ MINH (Ăn sáng/trưa)</h5>
              <p><b>07h00:</b> Đoàn trả phòng. Xe đưa đoàn đến nhà hàng dùng điêm tâm sáng. Sau đó khởi hành về lại Tp.HCM</p>
              <p><b>09h00:</b> Đoàn dừng chân tham quan Thác Voi Đà Lạt. Quý khách sẽ được len lõi theo những vách đá xuống chân thác ngắm bầy voi được tạo hóa dựng nên. Nơi đây có những tảng đá mang vóc dáng những chú voi thật đẹp.</p>
              <p><b>10h00:</b> Đoàn tiếp tục thăm viếng Chùa Linh Ẩn một trong “tứ Linh cổ tự của Đà Lạt”. Tại đây quý khách được chiêm bái tượng phật cao nhất Lâm Đồng hiện tại.</p>
              <p><b>11h30:</b> Đoàn dừng chân dùng cơm trưa tại nhà Tâm Châu – Lộc An, tự do thưởng thức trà, café miễn phí hay mua sắm đặc sản.</p>
              <p><b>19h00:</b> Đoàn về điểm trả khách ban đầu. HDV tạm biệt đoàn, kết thúc tour Tà Đùng 3 ngày 2 đêm, hẹn gặp lại đoàn trong thời gian gần nhất </p>
              
            </div>
          </div>
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

  },
   data() {
    return {
      selectedHotel: null
    }
  }
}

</script>

<style scoped>
img{
    size: 70%;
}
.stickyy {
  position: -webkit-sticky; 
  position: sticky;
  top: 100px;
}
#fontw{
  font-weight: 700;
  font-size: 30px;
  margin-left: 20px;
  
}
.price-display{
  font-size: 30px;
  font-weight: 600;
  color: #ff3131;
  border: rgb(148, 148, 148) 1px solid;
  border-radius: 5px;
  min-height: 125px;
  text-align: center;
  width: 200px;
}
b{
    color: #ff3131;
}
i{
    color: rgb(255, 166, 0);
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
  