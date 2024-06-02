<!-- src/components/Footer.vue -->
<template>
  <footer>
    <footer class="new_footer_area bg_color">
      <div class="new_footer_top">
        <div class="container">
          <div class="row">
            <div class="col-lg-3 col-md-6">
              <div class="f_widget company_widget wow fadeInLeft" data-wow-delay="0.2s" style="
                  visibility: visible;
                  animation-delay: 0.2s;
                  animation-name: fadeInLeft;
                ">
                <h3 class="f-title f_600 t_color f_size_18">Nhận tin</h3>
                <form action="#" class="f_subscribe_two mailchimp" method="post" novalidate="true" _lpchecked="1">
                  <input type="text" name="EMAIL" class="form-control memail" placeholder="Email" />
                  <button class="btn btn_get btn_get_two" type="submit">
                    Subscribe
                  </button>
                  <p class="mchimp-errmessage" style="display: none"></p>
                  <p class="mchimp-sucmessage" style="display: none"></p>
                </form>
              </div>
            </div>
            <div class="col-lg-3 col-md-6">
              <div class="f_widget about-widget pl_70 wow fadeInLeft" data-wow-delay="0.4s" style="
                  visibility: visible;
                  animation-delay: 0.4s;
                  animation-name: fadeInLeft;
                ">
                <h3 class="f-title f_600 t_color f_size_18">ĐẶT CHỖ</h3>
                <ul class="list-unstyled f_list">
                  <li><a href="#">Tel : 076 922 0162</a></li>
                  <li><a href="#">Fax : 076 922 0162</a></li>
                </ul>
              </div>
            </div>
            <div class="col-lg-3 col-md-6">
              <div class="f_widget about-widget pl_70 wow fadeInLeft" data-wow-delay="0.6s" style="
                  visibility: visible;
                  animation-delay: 0.6s;
                  animation-name: fadeInLeft;
                ">
                <h3 class="f-title f_600 t_color f_size_18">Địa chỉ</h3>
                <ul class="list-unstyled f_list">
                  <li>
                    <a href="#">HOTEL Mona Beach 319 C16 Lý Thường Kiệt Quận 11, TP.
                      HCM</a>
                  </li>
                </ul>
              </div>
            </div>
            <div class="col-lg-3 col-md-6">
              <div class="f_widget social-widget pl_70 wow fadeInLeft" data-wow-delay="0.8s" style="
                  visibility: visible;
                  animation-delay: 0.8s;
                  animation-name: fadeInLeft;
                ">
                <h3 class="f-title f_600 t_color f_size_18">Chia sẽ</h3>
                <div class="f_social_icon">
                  <a href="#" class="fab fa-facebook"></a>
                  <a href="#" class="fab fa-twitter"></a>
                  <a href="#" class="fab fa-linkedin"></a>
                  <a href="#" class="fab fa-pinterest"></a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="footer_bg">
          <div class="footer_bg_one"></div>
          <div class="footer_bg_two"></div>
        </div>
      </div>
      <div class="footer_bottom">
        <div class="container">
          <div class="row align-items-center">
            <div class="col-lg-6 col-sm-7"></div>
          </div>
        </div>
      </div>
    </footer>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
a {
  text-decoration: none;
}

body {
  background: #fbfbfd;
}

.new_footer_area {
  background: #fbfbfd;
}

.new_footer_top {
  padding: 120px 0px 270px;
  position: relative;
  overflow-x: hidden;
}

.new_footer_area .footer_bottom {
  padding-top: 5px;
  padding-bottom: 50px;
}

.footer_bottom {
  font-size: 14px;
  font-weight: 300;
  line-height: 20px;
  color: #7f88a6;
  padding: 27px 0px;
}

.new_footer_top .company_widget p {
  font-size: 16px;
  font-weight: 300;
  line-height: 28px;
  color: #6a7695;
  margin-bottom: 20px;
}

.new_footer_top .company_widget .f_subscribe_two .btn_get {
  border-width: 1px;
  margin-top: 20px;
}

.btn_get_two:hover {
  background: transparent;
  color: #5e2ced;
}

.btn_get:hover {
  color: #fff;
  background: #6754e2;
  border-color: #6754e2;
  -webkit-box-shadow: none;
  box-shadow: none;
}

a:hover,
a:focus,
.btn:hover,
.btn:focus,
button:hover,
button:focus {
  text-decoration: none;
  outline: none;
}

.new_footer_top .f_widget.about-widget .f_list li a:hover {
  color: #5e2ced;
}

.new_footer_top .f_widget.about-widget .f_list li {
  margin-bottom: 11px;
}

.f_widget.about-widget .f_list li:last-child {
  margin-bottom: 0px;
}

.f_widget.about-widget .f_list li {
  margin-bottom: 15px;
}

.f_widget.about-widget .f_list {
  margin-bottom: 0px;
}

.new_footer_top .f_social_icon a {
  width: 44px;
  height: 44px;
  line-height: 43px;
  background: transparent;
  border: 1px solid #e2e2eb;
  font-size: 24px;
}

.f_social_icon a {
  width: 46px;
  height: 46px;
  border-radius: 50%;
  font-size: 14px;
  line-height: 45px;
  color: #858da8;
  display: inline-block;
  background: #ebeef5;
  text-align: center;
  -webkit-transition: all 0.2s linear;
  -o-transition: all 0.2s linear;
  transition: all 0.2s linear;
}

.ti-facebook:before {
  content: "\e741";
}

.ti-twitter-alt:before {
  content: "\e74b";
}

.ti-vimeo-alt:before {
  content: "\e74a";
}

.ti-pinterest:before {
  content: "\e731";
}

.btn_get_two {
  -webkit-box-shadow: none;
  box-shadow: none;
  background: #5e2ced;
  border-color: #5e2ced;
  color: #fff;
}

.btn_get_two:hover {
  background: transparent;
  color: #5e2ced;
}

.new_footer_top .f_social_icon a:hover {
  background: #5e2ced;
  border-color: #5e2ced;
  color: white;
}

.new_footer_top .f_social_icon a+a {
  margin-left: 4px;
}

.new_footer_top .f-title {
  margin-bottom: 30px;
  color: #263b5e;
}

.f_600 {
  font-weight: 600;
}

.f_size_18 {
  font-size: 18px;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  color: #4b505e;
}

.new_footer_top .f_widget.about-widget .f_list li a {
  color: #6a7695;
}

.new_footer_top .footer_bg {
  position: absolute;
  bottom: 0;
  background: url("https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEigB8iI5tb8WSVBuVUGc9UjjB8O0708X7Fdic_4O1LT4CmLHoiwhanLXiRhe82yw0R7LgACQ2IhZaTY0hhmGi0gYp_Ynb49CVzfmXtYHUVKgXXpWvJ_oYT8cB4vzsnJLe3iCwuzj-w6PeYq_JaHmy_CoGoa6nw0FBo-2xLdOPvsLTh_fmYH2xhkaZ-OGQ/s16000/footer_bg.png") no-repeat scroll center 0;
  width: 100%;
  height: 266px;
}

.new_footer_top .footer_bg .footer_bg_one {
  background: url("https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEia0PYPxwT5ifToyP3SNZeQWfJEWrUENYA5IXM6sN5vLwAKvaJS1pQVu8mOFFUa_ET4JuHNTFAxKURFerJYHDUWXLXl1vDofYXuij45JZelYOjEFoCOn7E6Vxu0fwV7ACPzArcno1rYuVxGB7JY6G7__e4_KZW4lTYIaHSLVaVLzklZBLZnQw047oq5-Q/s16000/volks.gif") no-repeat center center;
  width: 330px;
  height: 105px;
  background-size: 100%;
  position: absolute;
  bottom: 0;
  left: 30%;
  -webkit-animation: myfirst 22s linear infinite;
  animation: myfirst 22s linear infinite;
}

.new_footer_top .footer_bg .footer_bg_two {
  background: url("https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhyLGwEUVwPK6Vi8xXMymsc-ZXVwLWyXhogZxbcXQYSY55REw_0D4VTQnsVzCrL7nsyjd0P7RVOI5NKJbQ75koZIalD8mqbMquP20fL3DxsWngKkOLOzoOf9sMuxlbyfkIBTsDw5WFUj-YJiI50yzgVjF8cZPHhEjkOP_PRTQXDHEq8AyWpBiJdN9SfQA/s16000/cyclist.gif") no-repeat center center;
  width: 88px;
  height: 100px;
  background-size: 100%;
  bottom: 0;
  left: 38%;
  position: absolute;
  -webkit-animation: myfirst 30s linear infinite;
  animation: myfirst 30s linear infinite;
}

@-moz-keyframes myfirst {
  0% {
    left: -25%;
  }

  100% {
    left: 100%;
  }
}

@-webkit-keyframes myfirst {
  0% {
    left: -25%;
  }

  100% {
    left: 100%;
  }
}

@keyframes myfirst {
  0% {
    left: -25%;
  }

  100% {
    left: 100%;
  }
}

.menu {
  position: relative;

  background: #e8e8f3;
  border-radius: 100%;
  cursor: pointer;
  box-shadow: 7px 7px 15px rgba(55, 84, 170, 0.15),
    -7px -7px 20px rgba(255, 255, 255, 1),
    inset 0px 0px 4px rgba(255, 255, 255, 0.2),
    inset 7px 7px 15px rgba(55, 84, 170, 0),
    inset -7px -7px 20px rgba(255, 255, 255, 0),
    0px 0px 4px rgba(255, 255, 255, 0);

  &::before,
  &::after {
    content: "";
    background: #c3c2c7;
    border-radius: 5px;
    width: 30px;
    height: 5px;
    position: absolute;
    right: 100px;
    transition: 0.2s ease;
    z-index: 1;
  }

  &::before {
    transform: rotate(0deg);
  }

  &::after {
    transform: rotate(-90deg);
  }

  &.open {
    opacity: 0.9;

    &::before {
      transform: rotate(45deg);
    }

    &::after {
      transform: rotate(-45deg);
    }

    .button {
      opacity: 1;
      pointer-events: auto;

      &:first-of-type {
        bottom: 40px;
        right: 70px;
      }

      &:nth-of-type(2) {
        bottom: 80px;
        transition-delay: 0.05s;
      }

      &:last-of-type {
        bottom: 40px;
        right: -70px;
        transition-delay: 0.1s;
      }
    }
  }
}

.button {
  padding: 30px;
  border-radius: 50%;
  cursor: pointer;
  background: #e8e8f3;
  position: absolute;
  bottom: 0;
  right: 0;
  opacity: 0;
  pointer-events: none;
  box-shadow: inherit;
  transition: 0.2s cubic-bezier(0.18, 0.89, 0.32, 1.28), 0.2s ease opacity,
    0.2s cubic-bezier(0.08, 0.82, 0.17, 1) transform;
  z-index: -1;

  &:hover {
    transform: scale(1.1);
  }

  &:first-of-type {
    background: url("https://assets.codepen.io/3537853/cam.svg") no-repeat 50%/50% #e8e8f3;
  }

  &:nth-of-type(2) {
    background: url("https://assets.codepen.io/3537853/img.svg") no-repeat 50%/ 50% #e8e8f3;
  }

  &:last-of-type {
    background: url("https://assets.codepen.io/3537853/music.svg") no-repeat 50% 45%/50% 45% #e8e8f3;
  }
}

/*************footer End*****************/
</style>
