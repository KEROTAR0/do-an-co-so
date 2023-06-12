<template>
  <compheader/>
  <compslider/>

    <div class="container ps-5 pe-5 mt-4">
      <div class="content">
        <h3>TOUR DU LỊCH ĐÀ LẠT - NGẮM HOA MÙA XUÂN</h3>
            
        <div>
          <div >                    
            <img src="../assets/images/Tour/tour-ngam-hoa-mua-xuan-da-lat.jpg" class="card-img-top" alt="...">
        </div>          
        <div class="d-flex justify-content-between">
          <div class="d-flex flex-column mb-3">
            <div class="p-2">Mã Tour: ZT0098</div>
            <div class="p-2">Thời gian: 4 ngày 3 đêm</div>
            <div class="p-2">Loại xe: Du lịch</div> 
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
                    <p>3.190.000đ</p>
                  </div>
                  <div v-if="selectedHotel === 'hotel2'">
                    <p>3.990.000đ</p>
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
              <h5>TP.HCM - ĐÀ LẠT - THÁC PONGOUR (Ăn sáng, trưa, chiều)</h5>
              <p><b>05h00:</b> Hướng dẫn viên công ty du lịch đón khách tại điểm hẹn, đoàn khởi hành chương trình tour Đà Lạt 4 ngày 3 đêm Tết 2023.Quý khách có thể nhìn ngắm cảnh sắc thiên nhiên mùa xuân trên đường đi</p>
              <p><b>07h30:</b> Đoàn ăn sáng tại nhà hàng trên đường đi. Đoàn cùng HDV giao lưu các trò chơi vui nhộn trên xe, cùng nghe về vùng đất có Đá 3 chồng, Suối Tiên, rừng Giá Tỵ, Madagui,…</p>
              <p><b>11h30:</b>  Đoàn ăn trưa tại Nhà hàng Tâm Châu Lộc An, quê hương của Vua Trà Việt Nam.</p>
              <p><b>14h30:</b> Quý khách dừng chân tham quan Thác Pongour, ngọn thác có chiều cao tới 40m, chảy qua 7 tầng đá phía dưới trước khi xuống được mặt hồ vì vậy mà thác Pongour còn có tên khác là "Thác bảy tầng".</p>
              <p><b>18h00:</b> Đoàn di chuyển về nhà hàng dùng bữa tối sau đó đến khách sạn nhận phòng và nghỉ ngơi. </p>
              <p><b>Tối:</b> Quý khách tự do khám phá phố núi về đêm. Thưởng thức các món đặc trưng của ẩm thực Đà Lạt như bánh tráng nướng, sữa đậu nành…</p>
        

              <h5 id="list-item-2">Ngày 2</h5>
              <h5>CHUỒN CHUỒN BISTRO – PUPPY FARM - BUFFET RAU (Ăn sáng, trưa, tối)</h5>
              <p><b>07h00:</b> Dùng buffet sáng tại tại nhà hàng, sau đó tiếp tục chương trình tham quan:</p>
              <p><b>08h00:</b> Tiếp tục tour Đà Lạt 4N3Đ, đoàn ghé thăm Chuồn Chuồn Bistro & Coffee. Không gian quán nằm bên cạnh rừng thông, phía trước là một con suối nhỏ bắc ngang khiến không gian quán cực kì thơ mộng. Khi lên tầng cao nhất của quán, quý khách sẽ được ngắm toàn cảnh thiên nhiên xanh mát. Không chỉ có vậy, nơi đây còn có nhiều tiểu cảnh cực hút mắt như hồ vô cực, hồ chuồn chuồn,...</p>
              <p><b>10h00:</b> Khởi hành tham quan Thiền Viện Trúc Lâm là thiền viện thuộc thiền phái Trúc Lâm Yên Tử, Nơi đây cũng là thiền viện lớn nhất Lâm Đồng, Từ trên chính điện nhìn xuống là quý khách sẽ được chiêm ngưỡng Hồ Tuyền Lâm, phong cảnh ở đây rất đẹp, hồ nước trong xanh in bóng rặng thông bên đồi Thanh Lương.</p>
              <p><b>11h30:</b> Đoàn dùng cơm trưa tại nhà hàng và xe đưa quý khách về khách sạn nghỉ ngơi.</p>
              <p><b>15h00:</b> Đoàn khởi hành tham quan nông trại cún Puppy Farm, quý khách có thể tham quan, vui chơi chụp ảnh cùng với những chú cún dễ thương được nuôi dưỡng bài bản, kết hợp tham quan những đồi hoa với nhiều loài hoa đua sắc, cho du khách cảm giác lạc vào không gian hoa bao la, bát ngát và quý khách có thể tham quan cả vườn dâu công nghệ cao, vườn cà chua cherry, dưa pepino, vườn xương rồng.</p>
              <p><b>17h30:</b> Đoàn di chuyển đến Đồi Robin Đà Lạt, từ đây quý khách có thể ngắm nhìn toàn cảnh thành phố Đà Lạt, ngắm nhìn voi với cảnh sắc thiên nhiên hùng vĩ. Sau đó đoàn dùng bữa tối với tiệc Buffet rau.</p>
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
              <p><b>Tối:</b> Quý khách tự do khám phá phố núi về đêm. Thưởng thức các món ngon tại Đà Lạt: Lẩu bò Ba Toa, bánh trắng nướng...</p>

              <h5 id="list-item-3">Ngày 3</h5>
              <h5>QUẢNG TRƯỜNG LÂM VIÊN - PHÂN VIỆN SINH HỌC – LANGBIANG (Ăn sáng, trưa)</h5>
              <p><b>07h00:</b> Đoàn khởi hành đi dùng buffet sáng.</p>
              <p><b>08h00:</b> Đoàn dừng chân tham quan Quảng Trường Lâm Viên, tại đây quý khách tha hồ check-in với biểu tượng của Đà Lạt: biểu tượng Hoa dã quỳ và Nụ hoa Atiso khổng lồ bằng kính.</p>
              <p><b>09h30:</b> Đoàn đến tham quan và tìm hiểu Phân Viện Sinh Học Đà Lạt. Toàn bộ bảo tàng được làm bằng đá, mang lối kiến trúc gothic kiếu Pháp với rất nhiều ô cửa trông giống hệt một tòa lâu đài nguy nga, cổ kính của châu Âu mang hơi thở huyền bí. Bảo tàng lưu giữ và bảo tồn nhiều nguồn gen quý qua các hiện vật vô cùng phong  phú, khu trưng bày xường sừng, mô hình các loài động vật quý hiếm như: voi, hổ, gấu, vượn…</p>
              <br>
              <p>Quý khách tiếp tục tham quan Lâu Đài Chocolate nằm trong khuôn viên nơi này. Đây là bảo tàng chocolate đầu tiên tại Việt Nam. Quý khách sẽ có được cảm giác mới mẻ khi biết được chocolate không chỉ là một món ăn mà còn là các tác phẩm nghệ thuật đẹp đến nao lòng. Tận mắt chứng kiến cảnh tạo chocolate nguyên chất. Tận tay trải nghiệm cách làm chocolate thủ công là món quà ý nghĩa dành tặng cho người thân và bạn bè.</p>
              <p><b>10h30:</b> Tham quan và mua sắm tại Cơ sở sản xuất mứt Đà Lạt. Quý khách được dùng nhiều loại mứt và trà atiso miễn phí tại đây.</p>
              <p><b>Trưa:</b> Đoàn dùng bữa trưa tại nhà hàng sau đó về lại khách sạn nghỉ ngơi.</p>
              <p><b>14h30:</b> Đoàn tham quan Nhà thờ Domaine de Marie còn được gọi với một cái tên khác là nhà thờ Vinh Sơn, đây là một ngôi nhà thờ nổi tiếng tại thành phố Đà Lạt. Tổng quan về kiến trúc của ngôi nhà thờ khá độc đáo, bên cạnh có kiến trúc gần giống nhà Rông truyền thống, thì khu vực phía sau là một khu vườn tuyệt đẹp và bình yên giữa lòng của ngôi nhà thờ.</p>
              <p><b>17h30:</b> Tiếp tục chương trình đoàn đến KDL LangBiang - ngọn núi cao nhất trên lâm viên cao nguyên. Quý khách có thể di chuyển bằng xe jeep chinh phục đỉnh núi Langbiang <i>(chi phí xe jeep tự túc)</i> tại đỉnh quý khách có thể ngắm nhìn toàn cảnh hồ suối vàng.</p>

              <p><b>Tối:</b> Quý khách tự do khám phá phố núi về đêm. Thưởng thức các món ngon tại Đà Lạt: Lẩu bò Ba Toa, Nướng ngói Cu Đức… <i>(bữa tối tự túc)</i></p>
              
              <h5 id="list-item-4">Ngày 4</h5>
              <h5>ĐÀ LẠT - TPHCM (Ăn sáng, trưa)</h5>
              <p><b>06h30:</b> Quý khách dùng điểm tâm sáng, trả phòng khách sạn. Xe đưa đoàn rời Đà Lạt về lại TP. HCM.</p>
              <p><b>08h00:</b> Quý khách tham quan và mua sắm tại chợ Đà Lạt sau đó đoàn lên xe rời Tp. Đà Lạt.</p>
              <p><b>11h00:</b> Dừng chân tại Lộc An thưởng thức Café miền cao nguyên miễn phí. Quý khách có thể mua đặc sản như: bơ, trà, café. </p>
              <p><b>11h30:</b> Đoàn dùng bữa trưa tại nhà hàng Tâm Châu Lộc An.</p>
              <p><b>18h30:</b> Về TP.HCM, hướng dẫn viên chào tạm biệt và hẹn gặp lại. Kết thúc chương trình tour Đà Lạt 4 ngày 3 đêm Tết 2023.</p>
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
  