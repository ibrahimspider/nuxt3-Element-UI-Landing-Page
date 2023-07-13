<template>
  <section>
    <div class="container">
      <h2>
        We are build awesome <br />
        marketing template
      </h2>
      <p>
        This is just a simple text made for this unique and awesome template,
        <br />
        you can replace it with any text.
      </p>
    </div>
    <!--  -->
    <div class="container">
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6"
          ><div class="grid-content ep-bg-purple">
            <el-button type="success" class="icon" :icon="Check" circle />
            <div>
              <a href="#" class="title">Grow Your Business</a>
              <p class="text-muted mt-3">
                The phrasal sequence of the is now so that many campaign and
                benefit
              </p>
              <el-link type="primary">Read More </el-link>
            </div>
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6"
          ><div class="grid-content ep-bg-purple">
            <el-button type="success" class="icon" :icon="Star" circle />
            <div>
              <a href="#" class="title">Grow Your Business</a>
              <p class="text-muted mt-3">
                The phrasal sequence of the is now so that many campaign and
                benefit
              </p>
              <el-link type="primary">Read More </el-link>
            </div>
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6"
          ><div class="grid-content ep-bg-purple">
            <el-button type="success" class="icon" :icon="Message" circle />
            <div>
              <a href="#" class="title">Grow Your Business</a>
              <p class="text-muted mt-3">
                The phrasal sequence of the is now so that many campaign and
                benefit
              </p>
              <el-link type="primary">Read More </el-link>
            </div>
          </div>
        </el-col>
        <el-col :xs="24" :sm="12" :md="12" :lg="6" :xl="6"
          ><div class="grid-content ep-bg-purple">
            <el-button type="success" class="icon" :icon="Edit" circle />
            <div>
              <a href="#" class="title">Grow Your Business</a>
              <p class="text-muted mt-3">
                The phrasal sequence of the is now so that many campaign and
                benefit
              </p>
              <el-link type="primary">Read More </el-link>
            </div>
          </div>
        </el-col>
      </el-row>
    </div>
  </section>
</template>

<script lang="ts" setup>
import {
  Check,
  Delete,
  Edit,
  Message,
  Search,
  Star,
} from "@element-plus/icons-vue";
</script>

<style scoped>
section {
  padding: 70px 0;
  text-align: center;
}
section h2 {
  letter-spacing: 0.5px;
  font-size: 32px;
  margin-bottom: 1.5rem;
}
section p {
  color: #8492a6;
  font-size: 16px;
  margin-bottom: 40px;
}
.el-row {
  margin-bottom: 20px;
}
.el-row:last-child {
  margin-bottom: 0;
}
.el-col {
  border-radius: 4px;
}

.grid-content {
  border-radius: 4px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px;
  border-radius: 10px;
  padding: 1.5rem;
  margin-bottom: 20px;
}
.icon {
  background: linear-gradient(45deg, #5329c4, #aa65e8) !important;
  height: 90px;
  width: 90px;
  color: #fff;
  font-size: 25px;
  margin-bottom: 30px;
}
section a {
  text-decoration: none;
}
section .title {
  color: #24272c;
  font-size: 18px;
  font-weight: bold;
  transition: all 200ms ease-in-out;
}
section .title:hover {
  color: #5329c4;
}
.mt-3 {
  margin-bottom: 20px;
}
</style>
