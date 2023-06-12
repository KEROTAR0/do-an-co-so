<template>
  <compheader/>
  <compslider/>

    <div class="container ps-5 pe-5 mt-4">
      <div class="content">
        <h3>LỊCH KHỞI HÀNH TOUR ĐÀ LẠT SĂN MÂY - THE BALI HILL</h3>
            
        <div>
          <div >                    
              <img src="../assets/images/Tour/tour-da-lat-san-may-the-bali-hill-3n3d-tu-tphcm.jpg" class="card-img-top" alt="...">
        </div>          
        <div class="d-flex justify-content-between">
          <div class="d-flex flex-column mb-3">
            <div class="p-2">Mã Tour: ZT0043</div>
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
                <div class="p-2">
                  <input type="radio" id="hotel3" value="hotel3" v-model="selectedHotel">
                  <label for="hotel3">Khách sạn 4 sao</label></div>
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
                    <p>2.490.000đ</p>
                  </div>
                  <div v-if="selectedHotel === 'hotel3'">
                    <p>2.990.000đ</p>
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
              <p><b>22h00:</b> Xe và HDV của công ty đón khách tại điểm hẹn (theo địa điểm hẹn trước). Bắt đầu chương trình Tour Đà Lạt 3 ngày 3 đêm Săn Mây - Samten Hill, trên xe HDV sinh hoạt chương trình tham quan và tổ chức các trò chơi vui nhộn. Quý khách nghỉ đêm trên xe để hôm sau có thể trải nghiệm trọn vẹn tour Đà Lạt săn mây.</p>
              
              <h5 id="list-item-2">Ngày 2</h5>
              <h5>CLOUD VIEW – ĐỒI CHÈ CẦU ĐẤT - QUẢNG TRƯỜNG LÂM VIÊN – PUPPY FARM (Ăn sáng, trưa)</h5>
              <p><b>05h00:</b> Đoàn ghé Cloud View – Thiên đường săn mây, đây là một trong những địa điểm săn mây đẹp nhất Đà Lạt. Đến đây bạn có thể ngồi xuống nhâm nhi tách cà phê nóng, ngắm những áng mây đang trôi phiêu bồng phía bên kia sườn núi và có cho mình thật nhiều tấm hình “ảo tung chảo” cùng khung cảnh thơ mộng nơi đây.</p>
              <p><b>06h30:</b> Dùng bữa sáng tại Café Panorama, ngắm toàn cảnh núi rừng Đà Lạt.</p>
              <p><b>08h30:</b> Điểm đến tiếp theo trong tour Săn Mây Đà Lạt 3N3Đ là Đồi Chè Cầu Đất. Toàn bộ đồi chè xanh rợp hiện ra giữa núi đồi Đà Lạt, trải dài trên khắp dải đồi rồi kéo dài như đến vô tận dưới nền trời trong xanh tạo nên một “bức tranh” vô cùng mãn nhãn. Sau đó quý khách có thể đi dạo thêm một chút để đến khám phá Đoàn tàu đỏ Phin Deli mới lạ và độc đáo, chắc chắn bạn sẽ có những tấm ảnh đẹp mê hồn với điểm này.</p>
              <p><b>10h00:</b> Ghé thăm chùa Linh Phước Đà Lạt hay còn được gọi là “Chùa Ve Chai” – ngôi chùa đạt nhiều kỷ lục nhất Việt Nam. Với nhiều công trình kiến trúc kỳ vỹ được làm từ hơn 5.000 mảnh ve chai. Tượng Phật Bà Quan Âm được kết bằng hàng ngàn đóa hoa bất tử. </p>
              <p><b>11h30:</b> Đoàn dùng bữa trưa tại nhà hàng, sau khi dùng bữa xong quý khách sẽ di chuyển đến khách sạn nhận phòng và nghỉ ngơi.</p>
              <p><b>15h30:</b> Đoàn đến check-in tại Quảng Trường Lâm Viên và chiêm ngưỡng 2 công trình nổi tiếng, được xem là biểu tượng của "Xứ sở sương mù" là biểu tượng Nụ Hoa Atiso và Hoa Dã Quỳ khổng lồ được làm bằng kính. Tại đây, quý khách vừa có thể chiêm ngưỡng 2 công trình này vừa có thể ngắm nhìn Hồ Xuân Hương thơ mộng sát bên.</p>
              <p><b>16h30:</b> Khởi hành tham quan Thiền Viện Trúc Lâm là thiền viện thuộc thiền phái Trúc Lâm Yên Tử, Nơi đây cũng là thiền viện lớn nhất Lâm Đồng, Từ trên chính điện nhìn xuống là quý khách sẽ được chiêm ngưỡng Hồ Tuyền Lâm với khung cảnh thanh bình, hồ nước trong xanh in bóng rặng thông bên đồi Thanh Lương Hoàng từ trên cao. <i>(Quý khách có thể đăng ký trải nghiệm đi đến Thiền Viện Trúc Lâm bằng cáp treo, chi phí cáp treo tự túc)</i>.</p>
              <p><b>17h30:</b> Đoàn di chuyển đến Đồi Robin dùng Buffet rau.</p>
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
              <p><b>Tối:</b> Quý khách tự do khám phá chợ âm phủ Đà Lạt hoặc tản bộ đạp xe quanh hồ Xuân Hương dưới tiết trời se lạnh của Đà Lạt.. </p>

              <h5 id="list-item-3">Ngày 3</h5>
              <h5>CHUỒN CHUỒN BISTRO & COFFEE – CHÙA LINH ẨN - MÊ LINH COFFEE - THIỀN VIỆN TRÚC LÂM (Ăn sáng, trưa, tối)</h5>
              <p><b>07h00:</b> DĐoàn dùng bữa sáng rồi tiếp tục hành trình khám phá Đà Lạt 3 ngày 3 đêm.</p>
              <p><b>08h00:</b> Bắt đầu ngày tham quan thứ 2 trong tour Đà Lạt 3N3Đ, đoàn đến với Chuồn Chuồn Bistro & Coffee. Trên đường đi đoàn sẽ đi qua Thung lũng hoa Tà Nung, 2 bên đường tại thung lũng đang nở rộ và ngập tràn trong sắc vàng của hoa Dã Quỳ. Đến Chuồn Chuồn Coffee, quán xuất hiện giữa sườn đồi, mang phong cách hiện đại, mới lạ, độc đáo cùng view nhìn ra rừng thông tuyệt đẹp sẽ mang đến cho bạn cảm giác yên bình giữa chốn núi rừng. Bên cạnh đó, quán còn xây dựng rất nhiều tiểu cảnh, góc check-in cực xinh như Hồ vô cực, tháp vọng cảnh, hồ chuồn chuồn,... và đặc biệt là cánh đồng hoa Dã Quỳ vàng ươm (tiểu cảnh mới tại đây) cho bạn check-in.</p>
              <p><b>10h00:</b> Quý khách dừng chân tại Mê Linh Coffee Garden, quán Cafe có Khung cảnh đẹp ngất ngây ở Đà Lạt, du khách thư thái trong một không gian vô cùng thoáng đãng xanh tươi bạt ngàn của rừng cà phê. Tầm nhìn 360 độ có một không hai tại đây, đến với Mê Linh Coffee Garden bạn không chỉ được ngắm nhìn khung cảnh tuyệt trần của nứi rừng, sông nước những dãy núi trập trùng mà quý khách còn có thể thưởng thức ly cà phê chồn chính hiệu nổi tiếng trứ danh <i>(Chi phí nước uống tự túc)</i>.</p>
              <p><b>11h30:</b> Đoàn dùng bữa trưa tại nhà hàng sau đó về lại khách sạn nghỉ ngơi.</p>
              <p><b>15h00:</b> Đoàn khởi hành tham quan trang trại cún Puppy Farm, Quý khách có thể tham quan, vui chơi chụp ảnh cùng với những chú cún dễ thương được nuôi dưỡng bài bản, kết hợp tham quan những đồi hoa với nhiều loài hoa đua sắc, cho du khách cảm giác lạc vào không gian hoa bao la, bát ngát và quý khách có thể tham quan cả vườn dâu công nghệ cao, vườn cà chua cherry, dưa pepino.</p>              
              <p><b>Tối:</b> Quý khách tự do khám phá và thưởng thức những món ăn trứ danh của Đà Lạt như: Lẩu bò Ba Toa, bánh ướt lòng gà, bánh căn Đà Lạt, bánh mì xíu mại, lẩu gà lá é, cơm lam gà nướng Đà Lạt, lẩu cá tầm Ngư Sơn, kem bơ, bánh tráng nướng,... <i>(bữa tối tự túc)</i>.</p>
              
              <h5 id="list-item-4">Ngày 4</h5>
              <h5>ĐÀ LẠT – THE BALI HILL – TP.HCM (Ăn sáng,trưa)</h5>
              <p><b>07h00:</b> Quý khách làm thủ tục trả phòng sau đó xe và HDV đưa đoàn dùng điểm tâm sáng tại The Bali Hill. Sau đó tham quan, chụp hình tại nơi đây với phong cách rừng mưa nhiệt đới xanh mát được phủ xanh bởi những cây xanh phủ rộng khắp kèm theo điểm nhấn của những loài hoa mang nét đặc trưng riêng của thành phố Đà Lạt. Tạo nên những góc check-in mang đậm nét văn hóa của “hòn đảo thiên đường nhiệt đới Bali”. Bên cạnh đó quý khách còn được thưởng thức những món nước trái cây mới lạ tất cả các trải nghiệm sẽ mang lại cho quý khách những kí ức vui vẻ của chuyến đi.</p>
              <p><b>09h30:</b> Trên đường về quý khách tham quan KDL Samten Hills Đà Lạt nởi đây là Không Gian Văn Hóa Tâm Linh Phật Giáo mới khánh thành của vùng núi cao nguyên nơi này. Đây là một công trình vĩ đại được tạo nên bởi các vị Lama sẽ tạo cho quý du khách cảm giác sáng khoái mới lạ mang âm hưởng của cao nguyên Tây Tạng và cả thấy nhẹ nhàng tâm hồn được thanh lọc khỏi bụi bẩn trần thế để cái tâm được an yên sau những bộn bề lo toan vất vả của cuộc sống hằng ngày. <i>(Chi phí chưa bao gồm)</i>.</p>
              <p><b>11h00:</b> Quý khách dừng chân dùng cơm trưa tại nhà hàng Tâm Châu – Lộc An, sau đó quý khách có thể tự do mua sắm đặc sản Trà – Cà phê.</p>
              <p><b>18h30:</b> Đoàn về tới Tp. Hồ Chí Minh, đưa quý khách về điểm đón ban đầu. Xe và HDV chia tay đoàn, kết thúc tour Đà Lạt Săn Mây 3N3Đ, hẹn gặp lại quý khách trong những chuyến đi tiếp theo.</p>
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
  