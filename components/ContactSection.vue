<template>
  <section>
    <div class="container">
      <div class="header">
        <h3>Get In Touch!</h3>
        <p>
          This is just a simple text made for this unique and awesome template,
          you can replace it with any text.
        </p>
      </div>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12">
          <div class="box">
            <input type="text" placeholder="Name" />
          </div>
          <div class="box">
            <input type="email" placeholder="Email" />
          </div>
          <div class="box">
            <input type="text" placeholder="Subject" />
          </div>
        </el-col>
        <el-col :xs="24" :sm="12">
          <div class="box">
            <textarea placeholder="Message"></textarea>
          </div>
        </el-col>
      </el-row>
      <div class="text-right">
        <button class="btn">Send Message</button>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style scoped>
section {
  padding: 70px 0;
}
.header {
  text-align: center;
}
.header h3 {
  letter-spacing: 0.5px;
  font-size: 32px !important;
  line-height: 1.6;
}
.header p {
  margin: auto;
  max-width: 600px;
  font-size: 18px;
  color: #8492a6;
  margin-bottom: 60px;
}
.box {
  margin-bottom: 20px;
}
textarea {
  width: 100%;
  height: 160px !important;
  padding: 5px 11px;
  border: none;
  box-shadow: 0 0 0 1px #dcdfe6;
  border-radius: 4px;
  color: #606266;
  outline: #409eff;
  transition: 200ms all ease-in-out;
}
textarea:focus {
  box-shadow: 0 0 0 1px #409eff;
}
textarea::placeholder {
  color: #939393;
}
.text-right {
  text-align: right;
}
input:focus {
  box-shadow: 0 0 0 1px #409eff;
}
input::placeholder {
  color: #939393;
}
input {
  width: 100%;
  padding: 5px 11px;
  border: none;
  box-shadow: 0 0 0 1px #dcdfe6;
  border-radius: 4px;
  color: #606266;
  outline: #409eff;
  transition: 200ms all ease-in-out;
  height: 40px;
}
.btn {
  margin-top: 20px;
  background: linear-gradient(45deg, #5329c4, #aa65e8);
  color: #fff;
  box-shadow: 0 3px 5px 0 rgba(83, 41, 196, 0.1);
  border-image: linear-gradient(to right, #5329c4, #aa65e8) 1;
  padding: 8px 20px;
  font-size: 18px;
  letter-spacing: 0.5px;
  transition: all 0.3s ease;
}
</style>
