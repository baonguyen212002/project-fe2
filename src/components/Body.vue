<!-- src/components/Body.vue -->
<template>
  <main>
    <div class="location">
      <div class="title">
        <h3><a>Điểm đến nổi bật</a></h3>
      </div>
      <div class="container-fluid">
        <div class="row">
          <div class="minip">
            <div class="mg">
              <div class="clr"></div>
              <div class="group">
                <span>Sapa</span>
              </div>
            </div>
            <div class="av" style="
              background-image: url('src/assets/img/sapa.png');
              background-size: 100% 100%;
              background-repeat: no-repeat;
            "></div>
            <div class="info">
              <name>...</name>
              <deets>
                369 › he/him<br />
                soccer player
              </deets>
            </div>
          </div>
          <div class="minip">
            <div class="mg">
              <div class="clr"></div>
              <div class="group">
                <span>PhúQuốc</span>
              </div>
            </div>
            <div class="av" style="background-image: url('src/assets/img/phuquoc.png')"></div>
            <div class="info">
              <name>jinkyu do</name>
              <deets>
                369 › he/him<br />
                soccer player
              </deets>
            </div>
          </div>
          <div class="minip">
            <div class="mg">
              <div class="clr"></div>
              <div class="group">
                <span>Thápchampa</span>
              </div>
            </div>
            <div class="av" style="background-image: url('src/assets/img/thapcham.png')"></div>
            <div class="info">
              <name>jinkyu do</name>
              <deets>
                369 › he/him<br />
                soccer player
              </deets>
            </div>
          </div>
        </div>
      </div>

    </div>
    <div class="content2">
      <div class="title">
        <h3><a>Cẩm nang du lịch</a></h3>
      </div>
      <div class="container">


        <div class="panel">
          <div class="ring">
            <div class="card card1"></div>
            <div class="border">
              <p class="title">Hoạt động đặc biệt</p>
              <div class="slide">
                <h6 class="para">Đi bộ trong rừng nguyên sinh</h6>
                <div class="line">
                  <h6 class="para">
                    Du khách có thể cắm trại và ngủ đêm trong rừng
                  </h6>
                </div>
              </div>
            </div>
          </div>
        </div>


        <div class="panel">
          <div class="ring">
            <div class="card card2"></div>
            <div class="border">
              <p class="title">Sắp xếp chuyến đi</p>
              <div class="slide">
                <h6 class="para">
                  Gói ưu đãi cho tour du lịch trong nước, quốc tế
                </h6>
                <div class="line">
                  <h6 class="para">
                    Khởi hành đúng lịch, tiết kiệm thời gian di chuyển, chi
                    phí tối ưu
                  </h6>
                </div>
              </div>
            </div>
          </div>
        </div>


        <div class="panel">
          <div class="ring">
            <div class="card card2"></div>
            <div class="border">
              <p class="title">Hướng dẫn nhiệt tình</p>
              <div class="slide">
                <h6 class="para">Đội ngũ hướng dẫn viên</h6>
              </div>
            </div>
          </div>
        </div>


        <div class="panel">
          <div class="ring">
            <div class="card card3"></div>
            <div class="border">
              <p class="title">Quản lý vị trí</p>
              <div class="slide">
                <h6 class="para">
                  Bạn sẽ có thể quản lý vị trí của mình một cách hiệu quả và
                  an toàn hơn trong suốt chuyến du lịch
                </h6>
              </div>
            </div>
          </div>
        </div>


      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "Body",
};
</script>

<style scoped>
main {
  font-family: Arial, Helvetica, sans-serif;
}

.title h3 {
  font-size: 25px;
  border-bottom: 0.1rem solid #000;
  font-weight: bold;
  padding: 0px;
  margin: 0px 150px 50px 150px;
  text-transform: uppercase;
}

.minip {
  width: 300px;
  height: 450px;
  margin: auto;
  background: #fb7272;
  position: relative;
  box-shadow: 0px 0px 5px var(--terracotta);
}

.minip .mg {
  width: 100%;
  height: 200px;
  position: absolute;
  top: 0px;
  left: 0px;
  display: grid;
  grid-template-columns: 250px 50px;
  grid-template-rows: 100px 150px;
  grid-template-areas:
    "clr group"
    "clr .....";
  transition: grid-template-columns 0.6s linear, grid-template-rows 0.6s linear;
}

.minip:hover .mg {
  grid-template-columns: 150px 150px;
  grid-template-rows: 50px 300px;
  transition: grid-template-columns 0.6s linear, grid-template-rows 0.6s linear;
}

.minip .mg .clr {
  grid-area: clr;
  background: #028a2b79;
}

.minip .mg .group {
  font: 10px/10px var(--mono);
  text-transform: uppercase;
  letter-spacing: 1px;
  writing-mode: vertical-lr;
  display: flex;
  align-items: center;
  justify-content: center;
}

.minip .mg .group span {
  display: block;
  transform: rotate(180deg);
  transition: transform 0.6s linear;
}

.minip:hover .mg .group span {
  transform: rotate(270deg);
  transition: transform 0.6s linear;
}

.minip .av {
  width: 200px;
  height: 350px;
  position: absolute;
  bottom: 0px;
  right: 0px;
  background: #000;
  background-position: top center;
  background-size: cover;
  transition: width 0.6s linear, height 0.6s linear;
}

.minip:hover .av {
  width: 300px;
  height: 400px;
  transition: width 0.6s linear, height 0.6s linear;
}

.minip .info {
  width: 160px;
  max-height: 100px;
  padding: 25px;
  position: absolute;
  bottom: 100px;
  left: 0px;
  background: #f7f6f6;
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-content: flex-start;
  transition: bottom 0.6s linear;
}

.minip:hover .info {
  bottom: 50px;
  transition: bottom 0.6s linear;
}

.minip .info name {
  display: block;
  font: 200 25px/30px var(--display);
  text-indent: -25px;
  letter-spacing: 1px;
  margin: 0px 0px 10px 25px;
}

.minip .info deets {
  font: 10px/15px var(--mono);
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* cdfvfdbfg */
.container {
  width: 100vw;
  max-width: 1200px;
  min-width: 1100px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.content2 {
  margin: 50px 0px;
}

.panel {
  height: 270px;
  width: 190px;
  position: relative;

  &:hover {
    .card {
      filter: blur(1.5px);
    }

    .card1 {
      background-size: 215% 135%;
    }

    .card2 {
      background-size: 115% 115%;
    }

    .card3 {
      background-size: 155% 115%;
    }

    .title {
      color: rgba(255, 255, 255, 0.2);
    }

    .border {
      border: 1px solid rgba(255, 255, 255, 1);
    }

    .slide {
      bottom: 0px;
    }

    .ring:before,
    .ring:after {
      transform: translateX(-50%) translateY(-50%) rotate(310deg);
    }
  }
}

.ring,
.card,
.border,
.slide,
.line {
  display: flex;
  justify-content: center;
  align-items: center;
}

.ring {
  color: #fffbf1;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
  font-size: 170px;
}

.card {
  background: #f0ead6;
  position: relative;
  transition: all 1s;
  height: 270px;
  width: 190px;
  border: 1px solid rgba(255, 255, 255, 1);
}

.card1 {
  background-image: url("https://assets.codepen.io/489403/brazil.jpg");
  background-repeat: no-repeat;
  background-size: 200% 120%;
}

.card2 {
  background-image: url("https://assets.codepen.io/489403/belize.jpg");
  background-repeat: no-repeat;
  background-size: 100% 100%;
}

.card3 {
  background-image: url("https://assets.codepen.io/489403/egypt.jpg");
  background-repeat: no-repeat;
  background-size: 140% 100%;
}

.ring:before,
.ring:after {
  content: "";
  padding: 0.7em 0.4em;
  position: absolute;
  left: 50%;
  width: 184%;
  top: 50%;
  display: block;
  border: 5px solid #50c9c3;
  border-radius: 50%;
  transition: transform 1s;
  transform: translateX(-50%) translateY(-50%) rotate(50deg);
}

.ring:before {
  border-color: rgb(235, 235, 235) rgb(235, 235, 235) rgba(0, 0, 0, 0) rgba(0, 0, 0, 0);
  z-index: -1;
}

.ring:after {
  border-color: rgba(0, 0, 0, 0) rgba(0, 0, 0, 0) rgb(235, 235, 235) rgb(235, 235, 235);
}

p {
  text-align: center;
  position: absolute;
}

.title {
  font-size: 36px;
  font-weight: 700;
  transition: all 1s;
  top: 0;
}

.para {
  bottom: 0;
  font-size: 16px;

  padding: 20px;
  margin: 0;
  text-align: center;
}

.border {
  position: absolute;
  border: 1px solid rgba(255, 255, 255, 0.5);
  height: 260px;
  width: 180px;
  transition: border 1s;
  overflow: hidden;
}

.slide {
  height: 260px;
  width: 180px;
  position: absolute;
  border: 1px solid black;
  bottom: -270px;
  background: rgba(0, 0, 0, 0.5);
  transition: bottom 1s;
  flex-direction: column;
}

.fa-plane {
  font-size: 16px;
}

/* location */
.location {
  background: #f4f4f7;
  padding: 50px 0px;
}
</style>
