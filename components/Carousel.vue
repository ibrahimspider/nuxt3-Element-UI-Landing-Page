<template>
  <el-carousel height="100vh">
    <el-carousel-item v-for="item in 4" :key="item">
      <div class="overlay">
        <img src="/img/bg.jpg" />
        <div class="overlay-box">
          <div class="content">
            <div>
              <h2>Get Better Results Today</h2>
              <p>
                This is just a simple text made for this unique and awesome
                template, you can replace it with any text.
              </p>
              <div>
                <el-button>Go Now</el-button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </el-carousel-item>
  </el-carousel>
  <div class="shape overflow-hidden text-white">
    <svg viewBox="0 0 2880 48" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path
        d="M0 48H1437.5H2880V0H2160C1442.5 52 720 0 720 0H0V48Z"
        fill="currentColor"
      ></path>
    </svg>
  </div>
</template>

<style scoped>
.shape {
  margin-top: -19px;
  position: relative;
  color: #fff;
  overflow: hidden;
}
svg {
  transform: scale(2);
  width: 100%;
  height: auto;
  transform-origin: top center;
}
.el-carousel__item img {
  width: 100%;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
.overlay {
  position: relative;
  height: 100%;
}
.overlay-box {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(45deg, #5329c4, #aa65e8);
  opacity: 0.8;
}
.overlay-box .content {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  padding: 0 10px;
}
.overlay-box .content div {
  max-width: 600px;
  margin: auto;
  text-align: center;
}
.overlay-box .content div h2 {
  font-size: 42px !important;
  letter-spacing: 0.2px;
  line-height: 1.5;
}
.overlay-box .content div p {
  font-size: 20px;
  letter-spacing: 0.5px;
  color: rgba(255, 255, 255, 0.5) !important;
}
@media (max-width: 768px) {
  .overlay-box .content div h2 {
    font-size: 34px !important;
  }
}
</style>
