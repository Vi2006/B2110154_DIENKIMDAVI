<template>
  <footer class="page-footer orange">
    <div class="container">
      <div class="row">
        <div class="col l6 s12">
          <h5 class="white-text">MORRA SHOP</h5>
          <p class="grey-text text-lighten-4">
            CÔNG TY TNHH QQR - Phân phối độc quyền thương hiệu nước hoa tại Việt
            Nam
          </p>
          <p class="grey-text text-lighten-4">
            Địa chỉ: 101 - 103Nguyễn Văn Linh, Đường 3 tháng 2, Quận Ninh Kiều,
            TP Cần Thơ
          </p>
          <p class="grey-text text-lighten-4">
            Hotline: 18005786-039567286-Email:MorraShop@gmail.com
          </p>
        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Chính Sách</h5>
          <ul>
            <li><a class="white-text" href="#!">Điều khoản dịch vụ</a></li>
            <li><a class="white-text" href="#!">Chính sách đổi trả</a></li>
            <li><a class="white-text" href="#!">Chính sách bảo mật</a></li>
            <li><a class="white-text" href="#!">Chính sách riêng</a></li>
          </ul>
        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Thông Tin Liên Hệ</h5>
          <ul>
            <li>
              <a class="white-text" href="#!">Facebook</a>
            </li>
            <li>
              <a class="white-text" href="#!">Instagram</a>
            </li>
            <li><a class="white-text" href="#!">Zalo</a></li>
            <li><a class="white-text" href="#!">Youtobe</a></li>
          </ul>
        </div>
      </div>
    </div>
    <!--    <div class="footer-copyright">
      <div class="container">
        Made by
        <a class="orange-text text-lighten-3" href="http://materializecss.com"
          >Materialize</a
        >
      </div>
    </div> -->
  </footer>
</template>

<script>
import axios from "axios";
import swal from "sweetalert2";
import store from "../../vuex/store";

export default {
  name: "AppFooter",

  data() {
    return {
      page: 0,
    };
  },

  computed: {
    user: function () {
      return store.getters.getUser;
    },

    login: function () {
      return store.getters.getLogin;
    },
  },
};
</script>
