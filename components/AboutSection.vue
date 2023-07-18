<template>
  <section>
    <div class="container">
      <el-row :gutter="20">
        <el-col :xs="24" :sm="24" :md="10" :lg="10" :xl="10">
          <img src="/img/about.png" alt="" />
        </el-col>
        <el-col :xs="24" :sm="24" :md="14" :lg="14" :xl="14">
          <div class="content">
            <h3 class="title">
              Unlimited Possibilities. <br />
              1st Class Templates.
            </h3>
            <p class="text-muted">
              This is just a simple text made for this unique and awesome
              template, you can replace it with any text.
            </p>
            <p class="text-muted">
              This is just a simple text made for this unique and awesome
              template, you can replace it with any text.
            </p>
            <a href="#" class="btn">Learn More</a>
          </div>
        </el-col>
      </el-row>
    </div>
  </section>
  <!--  -->
  <section>
    <div class="container">
      <el-row :gutter="20">
        <el-col :xs="24" :sm="24" :md="14" :lg="14" :xl="14">
          <div class="content flex">
            <h3 class="title">Why Choose us ?</h3>
            <p class="text-muted">
              This is just a simple text made for this unique and awesome
              template, you can replace it with any text.
            </p>
            <div class="flex-box">
              <div class="icon-box">
                <el-button type="primary" :icon="Edit" circle class="icon" />
              </div>
              <div>
                <h4>Fully Secured</h4>
                <p class="text-muted">
                  Moreover, in Latin only words at the beginning of sentences
                  are capitalized.
                </p>
              </div>
            </div>
            <div class="flex-box">
              <div class="icon-box">
                <el-button type="primary" :icon="Message" circle class="icon" />
              </div>
              <div>
                <h4>Best Performance</h4>
                <p class="text-muted">
                  If the fill text is intended to illustrate the characteristics
                  of sometimes.
                </p>
              </div>
            </div>
            <div>
              <a href="#" class="btn">Learn More</a>
            </div>
          </div>
        </el-col>
        <el-col :xs="24" :sm="24" :md="10" :lg="10" :xl="10">
          <div class="flex img">
            <img src="/img/laptop.png" class="laptop" />
          </div>
        </el-col>
      </el-row>
    </div>
  </section>
</template>

<script lang="ts" setup>
import { Message, Edit } from "@element-plus/icons-vue";
</script>

<style scoped>
section {
  background: #f2f6fa;
  padding: 70px 0;
  min-height: 100vh;
}
section img {
  width: 100%;
}
.content {
  padding-left: 20px;
}
section .title {
  font-size: 30px;
  line-height: 2.2;
}
section .text-muted {
  color: #8492a6;
  font-size: 16px;
  margin-bottom: 40px;
  line-height: 2.2;
  max-width: 500px;
}
section .btn {
  padding: 8px 20px;
  outline: none;
  text-decoration: none;
  font-size: 18px;
  letter-spacing: 0.5px;
  transition: all 0.3s ease;
  border-radius: 0;
  background: linear-gradient(45deg, #5329c4, #aa65e8);
  color: #fff;
  box-shadow: 0 3px 5px 0 rgba(83, 41, 196, 0.1);
  border-image: linear-gradient(to right, #5329c4, #aa65e8) 1;
}
.flex {
  height: 100%;
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.img {
  overflow: hidden;
}
.img .laptop {
  width: 200%;
}
.flex-box {
  display: flex;
  align-items: center;
}
.icon-box {
  padding-right: 10px;
}
.icon-box .icon {
  background: none;
  border: none;
  color: #5329c4;
  font-size: 35px;
}
@media (max-width: 768px) {
  section .title {
    font-size: 20px;
  }
  .img .laptop {
    width: 100%;
  }
  .img {
    margin-top: 70px;
  }
}
</style>
