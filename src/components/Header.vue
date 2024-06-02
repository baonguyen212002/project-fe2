<template>
  <header>
    <div class="banner-header">
      <div class="menu1">
        <nav
          class="navbar navbar-expand-lg navbar-light"
          :class="{ scrolled: isScrolled }"
          id="navbar"
        >
          <div class="container-fluid">
            <a class="navbar-brand" href="#">
              <img
                :src="logo"
                alt=""
                width="100"
                height="100"
                class="d-inline-block align-text-top"
              />
            </a>
            <button
              class="navbar-toggler"
              type="button"
              data-bs-toggle="collapse"
              data-bs-target="#navbarSupportedContent"
              aria-controls="navbarSupportedContent"
              aria-expanded="false"
              aria-label="Toggle navigation"
            >
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
              <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                  <a class="nav-link" href="#">Trang chủ</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Link</a>
                </li>
              </ul>
            </div>
            <div class="searchBox">
              <input
                class="searchInput"
                type="text"
                name=""
                placeholder="Search"
              />
              <button class="searchButton" href="#">
                <i class="fa-solid fa-magnifying-glass"></i>
              </button>
            </div>
          </div>
        </nav>
      </div>
    </div>
    <div class="menu2">
      <div class="overlay-content">
        <div class="content slide-in-left">
          <h1>Trãi nghiệm cùng chung tôi</h1>
          <p>
            Thiên đương nghĩ dưỡng cho mọi du khách. Quý khách sẽ được ngắm ánh
            bình minh và chiều hoang hôn tại khu nghi duong sang trọng
          </p>
        </div>
        <div class="Img">
          <img
            :src="cutoutImage"
            alt="Cutout"
            class="cutout-image slide-in-right"
          />
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import logo from "../assets/img/logo.png";
import cutoutImage from "../assets/img/cutout.png";
export default {
  name: "Header",
  data() {
    return {
      isScrolled: false,
      logo,
      cutoutImage,
      isContentVisible: false,
      isImageVisible: false,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      this.isScrolled = window.scrollY > 50; // Adjust this value as needed
    },
  },
};
</script>
<style scoped>
* {
  font-family: Arial, Helvetica, sans-serif;
}
/* Keyframes for sliding in from left */

.overlay-content {
  transform: translateY(-30%);
  display: flex;
  align-items: center; /* Vertical alignment */
  justify-content: space-between; /* Optional: Adjust based on your layout needs */
}

.content {
  margin-right: 20px; /* Add some space between the text and the image if needed */
  text-align: center;
  width: 50%;
  font-size: 18px;
  color: #264e86;
  margin-left: 30px;
}

.cutout-image {
  max-width: 100%; /* Adjust based on your image size requirements */
  height: auto;
  z-index: 1000;
}

.navbar-nav {
  margin: 0 auto; /* Center the navbar items */
}
a.nav-link {
  color: white !important;

  font-size: 20px;
  margin-left: 50px;
}
.banner-header {
  background-image: linear-gradient(
      rgba(15, 11, 212, 0.262),
      rgba(4, 3, 78, 0.303),
      /* Adjust color and opacity */ rgba(0, 0, 0, 0.5)
        /* Adjust color and opacity */
    ),
    url("src/assets/img/banner.jpg");

  height: 150vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: 100% 200vh;
  position: relative;
}

.searchBox {
  transform: translateX(50%);
  background: #bababb;
  margin: 0 200px;
  border-radius: 40px;
  padding: 10px;
}

.searchBox:hover > .searchInput {
  width: 240px;
  padding: 0 6px;
}

.searchBox:hover > .searchButton {
  background: rgb(12, 12, 12);
  color: #f6f7f9;
}

.searchButton {
  color: rgb(235, 232, 232);
  float: right;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: #2f3640;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.4s;
}

.searchInput {
  border: none;
  background: none;
  outline: none;
  float: left;
  padding: 0;
  color: rgb(13, 12, 12);
  font-size: 16px;
  transition: 0.4s;
  line-height: 40px;
  width: 0px;
}
.menu1 {
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 1000; /* Đảm bảo thanh menu luôn ở trên các phần tử khác */
}

.navbar {
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Thêm bóng cho thanh menu */
}
.navbar {
  transition: background-color 0.3s ease;
}

/* Navbar styles when scrolled */
.navbar.scrolled {
  background-color: rgb(158, 144, 117) !important;
}
a.navbar-brand {
  margin-left: 38vh;
}
</style>
