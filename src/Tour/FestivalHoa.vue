<template>
  <compheader/>
  <compslider/>

    <div class="container ps-5 pe-5 mt-4">
      <div class="content">
        <h3>LỊCH KHỞI HÀNH TOUR FESTIVAL HOA ĐÀ LẠT 2023</h3>
            
        <div>
          <div >                    
            <img src="../assets/images/Tour/tour-du-lich-festival-hoa-da-lat.jpg" class="card-img-top" alt="...">
        </div>          
        <div class="d-flex justify-content-between">
          <div class="d-flex flex-column mb-3">
            <div class="p-2">Mã Tour: ZT0033</div>
            <div class="p-2">Thời gian: 3 ngày 3 đêm</div>
            <div class="p-2">Loại xe: Giường nằm/ ghế ngã</div> 
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
                    <p>1.890.000đ</p>
                  </div>
                  <div v-if="selectedHotel === 'hotel2'">
                    <p>2.490.000đ</p>
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
              <p><b>22h00:</b> Xe và HDV của công ty đón khách tại điểm hẹn (theo địa điểm hẹn trước). Đoàn bắt đầu hành trình tour Festival Hoa Đà Lạt 2023, trên xe HDV sẽ tổ chức hoạt náo, các hoạt động giao lưu. Quý khách nghỉ đêm.</p>
              
              <h5 id="list-item-2">Ngày 2</h5>
              <h5>CLOLD VIEW - ĐỒI CHÈ CẦU ĐẤT – F CÁNH ĐỒNG HOA - QUẢNG TRƯỜNG LÂM VIÊN (Ăn sáng, trưa)</h5>
              <p><b>05h00:</b> Quý khách đến địa điểm đầu tiên là Cloud View hay còn gọi là “Thiên Đường Săn Mây”, đây được xem là “đặc sản du lịch” tại Đà Lạt. Mọi người nói với nhau rằng: du lịch Đà Lạt mà chưa đến địa điểm này thì coi như bạn chưa đến đây. Bởi tại đây, quý khách có thể vừa sân mây vừa thưởng thức một tách trà nóng hay ly cà phê nóng tận hưởng không khí se lạnh của khí trời Đà Lạt lúc bình minh. Đặc biệt hơn hết mọi người sẽ có những bức ảnh “check in” cùng mây vô cùng thơ mộng.</p>
              <p><b>06h30:</b> Đoàn tiếp tục đến với Café Panorama một quán cà phê mộng mơ với view toàn cảnh thành phố Đà Lạt từ trên cao. Quý khách sẽ được dùng những món điểm tâm sáng nhẹ nhàng kết hợp cùng cà phê hoặc trà theo yêu cầu của mọi người. Bữa sáng đầu tiên của mọi người trong đoàn tại Đà Lạt càng trở nên đặc biệt khi thoải mái dùng bữa trong khung cảnh Đà Lạt thơ mộng vào buổi sớm ban mai.</p>
              <p><b>08h30:</b> Đoàn khởi hành tham quan Đồi Chè Cầu Đất với những hàng chè hiện ra trong khung cảnh thiên nhiên hài hòa, giữa màu xanh dương của bầu trời kết hợp với hình ảnh núi đồi rợp lên một màu xanh lá cây cối. Không gian đồi chè hiện lên vẻ đẹp bạt ngàn của những hàng chè tiếp nối nhau không có điểm kết thúc tạo nên một bức tranh phong cảnh đẹp tuyệt vời. Tiếp nối hành trình, đoàn sẽ đến với địa điểm hot nhất Đà Lạt gần đây là đoàn tàu đỏ Phin Deli. Quý khách sẽ được check in cùng với đoàn tàu đỏ vô cùng đặc sắc như tái hiện lại khung cảnh những năm 80. </p>
              <p><b>10h00:</b> Tiếp tục tham quan chùa Linh Phước hay còn được gọi là “Chùa Ve Chai” – ngôi chùa đạt nhiều kỷ lục nhất Việt Nam. Với nhiều công trình kiến trúc kỳ công được làm từ hơn 5.000 mảnh ve chai. Tượng Phật Bà Quan Âm được kết bằng hàng ngàn đóa hoa bất tử. Ngôi chùa mang vẻ đẹp hoài cổ sẽ rất thích hợp với những người yêu thích tìm kiếm sự bình an trong tâm hồn.</p>
              <p><b>11h30:</b> Quý khách dùng bữa trưa tại nhà hàng, sau đó đoàn về khách sạn nhận phòng và nghỉ ngơi.</p>
              <p><b>14h30:</b> Quý khách tham quan tại cánh đồng hoa nằm ẩn mình trong thung lũng bên sườn đồi cạnh đèo Mimosa, với không gian xanh mát của những đồi thông phía dưới là những cánh đồng hoa đang thi nhau nở rộ dưới một vùng trời tuyệt đẹp mang đậm chất Đà lạt theo từng mùa hoa.</p>
              <p><b>16h00:</b> Xe đưa quý khách đi tham quan Quảng Trường Lâm Viên, đây là điểm tham quan chưa bao giờ hết hot tại Đà Lạt. Tại đây Quý khách được chiêm ngưỡng biểu tượng Hoa Dã Quỳ và Nụ Hoa Atiso khổng lồ được làm bằng kính. Quý khách có thể vừa chụp hình vừa ngắm nhìn Hồ Xuân Hương Đà Lạt thơ mộng. Quý khách chụp hình với khinh khí cầu tại sự kiện khinh khí cầu Lễ hội Festival hoa Đà Lạt 2022.</p>
              <p><b>17h00:</b> Quý khách trải nghiệm khinh khí cầu, ngắm nhìn TP. Đà Lạt từ trên cao, thưởng ngoạn vẻ đẹp của hồ Xuân Hương mờ ảo lung linh và ngắm nhìn Đà Lạt hoàng hôn khi ánh chiều tà dần buôn xuống và nhìn từ xa dãy núi Langbiang thơ mộng. Đây sẽ là trải nghiệm mới mẻ khi quý du khách đến Đà Lạt mộng mơ vì lần đầu tiên tổ chức tại Đà Lạt. <i>(Chi phí tự túc)</i>.</p>
              <p><b>Tối:</b> Quý khách tự do khám phá và thưởng thức ẩm thực tại chợ Đà Lạt với những món đặc sản: bánh tráng nướng, lẩu bò ba toa, Nem Nướng... <i>(Ăn tối tự túc)</i>. Hoặc tự do tham gia chương trình tổng kết lễ bế mạc Festival hoa Đà Lạt 2022 và Chương trình nghệ thuật Chào năm mới 2023. </p>

              <h5 id="list-item-3">Ngày 3</h5>
              <h5>CHUỒN CHUỒN BISTRO – THUYỀN VIỆN TRÚC LÂM - PUPPY FARM – BUFFET RAU (Ăn sáng, trưa, tối)</h5>
              <p><b>07h00:</b> Dùng buffet sáng tại tại nhà hàng, sau đó tiếp tục chương trình tham quan:</p>
              <p><b>08h00:</b> Quý khách tiếp tục tham quan Chuồn Chuồn Bistro, địa điểm này là sự kết hợp giữa thiên nhiên tươi mát và phong cách thiết kế hiện đại mang phong cách mới lạ, độc đáo xuất hiện giữa thiên nhiên Đà Lạt. Mọi người trong đoàn sẽ được chiêm ngưỡng cánh rừng thông tuyệt đẹp. Nổi bật nhất tại đây phải kể đến tháp vọng cảnh nhiều tầng có view 360 độ. Thêm một góc sống ảo cực chill tại đây chính là hồ vô cực, tiếp đến là hồ chuồn chuồn thơ mộng nằm ngay dưới chân đồi, xung quanh hồ được trồng nhiều loài hoa tràn ngập sắc màu tạo nên không gian tươi mát, dễ chịu. Chắc chắn nơi đây sẽ không khiến bạn thất vọng bởi vẻ đẹp đặc sắc của nó.</p>
              <p><b>10h00:</b> Cả đoàn khởi hành tham quan Thiền Viện Trúc Lâm là thiền viện thuộc thiền phái Trúc Lâm Yên Tử. Thiền viện nằm ẩn mình trong phong cảnh núi non trùng điệp, tạo nên khung cảnh thanh tịnh khi mọi người đặt chân đến đây. Từ trên chính điện nhìn xuống, quý khách sẽ được chiêm ngưỡng Hồ Tuyền Lâm, với mặt hồ trong xanh in bóng rặng thông bên đồi Thanh Lương.</p>
              <p><b>11h30:</b> Đoàn dùng cơm trưa tại nhà hàng và xe đưa quý khách về khách sạn nghỉ ngơi.</p>
              <p><b>15h00:</b> Quý khách khởi hành tham quan trại cún Puppy Farm địa điểm đặc biệt dành cho team yêu thích động vật. Quý khách có thể tham quan, vui chơi và chụp ảnh cùng với những chú cún siêu dễ thương và thân thiện. Mọi người có thể đi dạo cùng những chú cún trên những đồi hoa sặc sỡ. Hay đơn giản hơn, du khách có thể tận hưởng cảm giác yên bình ngắm nhìn khung cảnh thiên nhiên tại Puppy Farm. Đặc biệt, quý khách có thể tham quan vườn dâu công nghệ cao, vườn cà chua cherry, dưa pepino cực kỳ độc đáo.</p>
              <p><b>17h30:</b> Đoàn di chuyển đến Đồi Robin được mệnh danh là nóc nhà trên cao của Đà Lạt. Khi phóng tầm nhìn ra xa, mọi người sẽ thu toàn bộ hình ảnh thành phố Đà Lạt vào trong tầm mắt, cùng cảnh sắc hùng vĩ của thiên nhiên Việt Nam mình. Sau đó cả đoàn dùng đại tiệc Buffet rau .</p>
              <div class="bor-der"><b>Thực đơn tham khảo:</b>
                <ol class="list-group list-group-numbered">
                  <li class="list-group-item">Buffet rau không giới hạn:
                    <div class="d-flex flex-column mb-3">
                      <div class="p-2">+ 15 loại rau đặc trưng của Đà Lạt dùng kèm lẩu.</div>
                      <div class="p-2">+ Bún & mì vàng.</div>
                      <div class="p-2">+ Trà atiso.</div>
                    </div>
                  </li>
                  <li class="list-group-item">Set thức ăn với lẩu tặng kèm: Thịt nai, thịt bò úc, trứng gà, nạc dăm, ức gà, bò viên, mực, tôm, nghêu lụa, cá diêu hồng, vây cá hồi, giò sống, thanh cua, nấm đùi gà, nấm bào ngư, nấm đông cô, nấm kim châm.</li>
                  <li class="list-group-item">Gà lắc ngũ cốc</li>
                  <li class="list-group-item">Cơm chiên Dương Châu</li>
                  <li class="list-group-item">Trái cây</li>

                </ol>
              </div>
              <p><b>Tối:</b> Quý khách tự do khám phá phố núi về đêm. Thưởng thức các món ngon tại Đà Lạt: Lẩu bò Ba Toa, bánh trắng nướng, kem bơ…</p>
              
              <h5 id="list-item-4">Ngày 4</h5>
              <h5>ĐÀ LẠT – THÁC PONGOUR – TP.HCM (Ăn sáng, ăn trưa)</h5>
              <p><b>07h00:</b> Quý khách làm thủ tục trả phòng, dùng điểm tâm sáng sau đó tiếp tục tham quan trên đường về.</p>
              <p><b>09h30:</b> Quý khách dừng chân tham quan Thác Pongour hay còn được gọi là "Thác Bảy Tầng" với độ cao hơn 40m đổ qua 7 tầng đá. Vẻ đẹp đặc biệt của dòng thác nằm ở hệ thống các bậc đá bằng phẳng, xếp thành lớp tuy không theo bất cứ một trật tự nào nhưng đã “xé” nguồn nước thành hàng trăm dòng nhỏ, tạo thành những thảm nước tung bọt trắng xóa, hùng vĩ. Bên dưới thác là một mặt hồ rộng thênh thang, yên bình với rất nhiều tảng đá nhấp nhố giữa dòng nước.</p>
              <p><b>12h00:</b> Quý khách dừng chân dùng cơm trưa tại nhà hàng Tâm Châu – Lộc An, sau đó quý khách có thể tự do mua sắm đặc sản Trà – Cà phê</p>
              <p><b>18h30:</b> Đoàn về ,xe và HDV đưa đoàn về điểm đón ban đầu. Kết thúc tour Festival Hoa Đà Lạt, hẹn gặp tại quý khách trong những chương trình tour tiếp theo.</p>
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
  