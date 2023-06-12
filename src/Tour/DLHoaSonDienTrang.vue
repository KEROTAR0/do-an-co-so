<template>
  <compheader/>
  <compslider/>

    <div class="container ps-5 pe-5 mt-4">
      <div class="content">
        <h3>LỊCH KHỞI HÀNH TOUR ĐÀ LẠT SĂN MÂY - THE BALI HILL</h3>
            
        <div>
          <div >                    
            <img src="../assets/images/Tour/tour-hoa-son-dien-trang-da-lat.jpg" class="card-img-top" alt="...">
        </div>          
        <div class="d-flex justify-content-between">
          <div class="d-flex flex-column mb-3">
            <div class="p-2">Mã Tour: ZT0070</div>
            <div class="p-2">Thời gian: 4 ngày 3 đêm</div>
            <div class="p-2">Loại xe: Otô</div> 
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
                    <p>2.190.000đ</p>
                  </div>
                  <div v-if="selectedHotel === 'hotel2'">
                    <p>3.590.000đ</p>
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
              <a class="list-group-item list-group-item-action" href="#list-item-4">Ngày 4</a>
            </div>
          </div>
          <div class="col-8">
            <div data-bs-spy="scroll" data-bs-target="#list-example" data-bs-smooth-scroll="true" class="scrollspy-example" tabindex="0">
              <h5 id="list-item-1">Ngày 1</h5>
              <h5>TP.HCM - ĐÀ LẠT - THÁC PONGOUR (Ăn sáng, trưa, chiều)</h5>
              <p><b>05h30:</b> Hướng dẫn viên du lịch đón khách tại điểm hẹn, đoàn khởi hành đi Đà Lạt, bắt đầu TOUR ĐÀ LẠT - HOA SƠN ĐIỀN TRANG - 4N3Đ.</p>
              <p><b>07h30:</b> Đoàn ăn sáng tại nhà hàng trên đường đi. Đoàn cùng HDV giao lưu các trò chơi vui nhộn trên xe, cùng nghe về vùng đất có Đá 3 chồng, rừng Giá Tỵ, Suối Tiên, Madagui,…</p>
              <p><b>11h30:</b> Đoàn ăn trưa tại Nhà hàng Tâm Châu Lộc An, quê hương của Vua Trà Việt Nam.</p>
              <p><b>14h30:</b> Quý khách dừng chân tham quan Thác Pongour hay còn được gọi là "Thác Bảy Tầng" hay “Nam Phương Đệ Nhất”  thác với độ cao hơn 40m đổ qua 7 tầng đá. Vẻ đẹp đặc biệt của dòng thác nằm ở hệ thống các bậc đá bằng phẳng, xếp thành lớp tuy không theo bất cứ một trật tự nào nhưng đã “xé” nguồn nước thành hàng trăm dòng nhỏ, tạo thành những thảm nước tung bọt trắng xóa, hùng vĩ. Bên dưới thác là một mặt hồ rộng thênh thang, yên bình với rất nhiều tảng đá nhấp nhố giữa dòng nước.</p>
              <p><b>16h00:</b> Đoàn dừng chân tham quan Quảng trường Lâm Viên. Chụp ảnh đoàn lưu niệm tại biểu tượng Hoa Dã Quỳ của Đà Lạt.</p>
              <p><b>17h00:</b> Đoàn dùng cơm chiều và về nhận phòng, khám phá chợ Đà Lạt về đêm, thưởng thức các món nướng trong không khí lạnh.</p>
                            
              <h5 id="list-item-2">Ngày 2</h5>
              <h5>HOA SƠN ĐIỀN TRANG - CÀ PHÊ MÊ LINH (Ăn sáng, trưa, chiều)</h5>
              <p><b>07h00:</b> Đoàn khởi hành đi dùng buffet sáng.</p>
              <p><b>08h30:</b> Sau khi chinh phục con đèo Tà Nung mệnh danh là “Con đường tơ lụa Đà Lạt” tuyệt đẹp, ngắm nhìn hoa anh đào nở giữa rừng thông,quý khách dừng chân tham quan Mê Linh Coffee Garden. Tại đây, quý khách có thể tham quan và tìm hiểu cách thức sản xuất cà phê chồn Đà Lạt trực tiếp hay quý khách có thể thưởng thức ly cafe thơm ngon và ngắm nhìn toàn cảnh hồ Đập Cam Ly thơ mộng. Quý khách có thể mua những sản phẩm dệt tơ tằm tại đây. Nêu may mắn vào những tuần có sẽ có hoa Hướng Dương hoặc hoa Cải Trắng nở rộ quý khách có thể tham quan <i>(Phi phí tự tuc: 10.000đ/khách)</i>.</p>
              <p><b>10h00:</b> Đoàn tiếp tục tham quan “Hoa Sơn Điền Trang”, được giới trẻ lùng sục check in cho ra những “ bức ảnh lung linh, huyền ảo tuyệt với” với những cảnh được cho hot nhất 2018: Bàn tay phật khổng lồ hay còn gọi là bàn tay may mắn, cánh đồng tam giác mạch, khu vườn hồng cổ sapa, hồ thác nước, tiểu cảnh quanh hồ, con đường hoa đào Nhật Bản (được nhập nguyên cây lớn từ Nhật), khu nhà gỗ trên cây.</p>
              <p><b>11h30:</b> Đoàn dùng buffet rau tại đồi Robin Đà Lạt. Quý khách thưởng thức nhiều loại rau tại đây.</p>
              <p><b>15h30:</b> Tham quan Đà Lạt View - một cổng trời ngay trung tâm thành phố Đà Lạt. Với vị trí thuận lợi, view quán cafe từ trên cao và nhìn toàn cảnh rừng thông vô cùng lãng mạn.</p>
              <p><b>16h00:</b> Quý khách tiếp tục tham quan King Palace hay thường gọi là “Dinh 1 Đà Lạt”. Đây là Dinh thự của vị vua cuối cùng triều Nguyễn : vua Bảo Đại. Ngôi nhà chính mang kiến trúc Pháp cổ điển, bên trong có trưng bày tượng sáp vua Bảo Đại và hoàng hậu Nam Phương. Ngoài ra khung cảnh nơi đây như một phần thu nhỏ của nước pháp.</p>
              <p><b>17h30:</b> Đoàn ăn cơm chiều tại nhà hàng.</p>
              <p><b>Tối:</b> Quý khách tự do khám phá phố núi về đêm.</p>

              <h5 id="list-item-3">Ngày 3</h5>
              <h5>KING PALACE - LANGBIANG (Ăn sáng, trưa, chiều)</h5>
              <p><b>07h30:</b> Đoàn khởi hành dùng điểm tâm sáng.</p>
              <p><b>09h00:</b> Đoàn tham quan nhà ga xe lửa Đà Lạt, một trong những nhà ga đẹp nhất Đông Dương với đường xe lửa bánh răng độc đáo nhất thế giới.</p>
              <p>Đoàn có thể mua vé đi trên chuyến xe lửa xưa để gợi nhớ về Đà Lạt mộng mơ một thời <i>(chi phí tự túc)</i> để đến với chùa Linh Phước Đà Lạt (chùa Ve Chai) – có tượng rồng được đắp bằng vỏ 12.000 vỏ chay bia, ngắm nhìn tượng phật quan âm kết bằng hoa Bất Tử.</p>
              <p><b>10h30:</b> Đoàn khởi hành tham quan vườn hoa Cẩm Tú Cầu. Quý khách sẽ lạc vào vườn hoa vô cùng lãng mạn giống như trong chuyện cổ tích.</p>
              <p><b>12h00:</b> Đoàn ăn cơm trưa tại nhà hàng</p>
              <p><b>15h00:</b> Tham quan và mua sắm tại cở sở sản xuất mứt Đà Lạt. Quý khách được dùng nhiều loại mứt và trà atiso miễn phí tại đây.</p>              
              <p><b>16h30:</b> Khởi hành đến núi Lang Biang ngọn núi cao nhất trên lâm viên cao nguyên.</p>              
              <div class="d-flex flex-column mb-3">
                <div class="p-2">+ Nghe truyền thuyết về dân tộc Lạch với chuyện tình chàng Lang và nàngBiang.</div>
                <div class="p-2">+ Chinh phục đỉnh LangBiang cao hơn 2.000m, quý khách có thể lên đỉnh rađa bằng xe uwoat <i>(chi phí tự túc)</i>. Ðứng ở đây có thể ngắm trọn vẹn thành phố Ðà Lạt mộng mơ, hiện ra như một bức tranh thủy mặc, phía tây là hồ Dankia-Suối Vàng trông như một tấm lụa đào khổng lồ nổi bật giữa màu xanh bạt ngàn của núi đồi.</div>
              </div>
              <p><b>18h00:</b> Đoàn dùng cơm tối và tự do khám phá chợ Đà Lạt và mua đặc sản về làm quà.</p>              
                            
              <h5 id="list-item-4">Ngày 4</h5>
              <h5>ĐÀ LẠT - TP.HCM (Ăn sáng, trưa, chiều)</h5>
              <p><b>07h00:</b> Quý khách dùng điểm tâm sáng, trả phòng khách sạn. Xe đưa đoàn rời Đà Lạt về lại TP. HCM.</p>
              <p><b>08h00:</b> Quý khách tham và mua sắm tại chợ Đà Lạt.</p>
              <p><b>11h00:</b> Dừng chân tại Lộc An thưởng thức Café miền cao nguyên miễn phí. Quý khách có thể mua đặc sản như: bơ, trà, café. </p>
              <p><b>11h30:</b> Đoàn ăn trưa tại Tâm Châu, Lộc An.</p>
              <p><b>18h00:</b> Về TP.HCM, kết thúc tour du lịch Đà Lạt - Hoa Sơn Điền Trang, chào tạm biệt quý khách và hẹn gặp lại.</p>
              <p><b>Lưu ý:</b> Thứ tự tham quan các điểm có thể thay đổi để phù hợp với điều kiện thực tế của chương trình nhưng vẫn đảm bảo đi đủ các  điểm tham quan trong chương trình.</p>
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
  