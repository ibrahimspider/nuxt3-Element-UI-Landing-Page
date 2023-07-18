<template>
  <section>
    <div class="container">
      <div class="header">
        <h3>
          Choose our package <br />
          & Active to premium
        </h3>
        <p>
          This is just a simple text made for this unique and awesome template,
          you can replace it with any text.
        </p>
      </div>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="8" v-for="packagee in packages">
          <div class="grid-content">
            <div class="flex">
              <div>
                <el-button class="icon" :icon="Star" circle />
                <h3>{{ packagee.title }}</h3>
                <p>
                  $<span>{{ packagee.price }}</span
                  >/month
                </p>
              </div>
            </div>
            <div class="features">
              <h5>Pricing Features:</h5>
              <p class="list" v-for="list in packagee.features">
                <el-button class="features-btn" :icon="Check" circle />{{
                  list
                }}
              </p>
            </div>
          </div>
        </el-col>
      </el-row>
    </div>
  </section>
</template>

<script setup>
import {
  Check,
  Delete,
  Edit,
  Message,
  Search,
  Star,
} from "@element-plus/icons-vue";

const packages = [
  {
    icon: "Check",
    title: "Basic",
    price: "19",
    features: [
      " Full Access",
      "Source Files",
      "Free Appointments",
      "Enhanced Security",
    ],
  },
  {
    icon: "Star",
    title: "Premium",
    price: "39",
    features: [
      " Full Access",
      "Source Files",
      "Free Appointments",
      "Enhanced Security",
    ],
  },
  {
    icon: "Message",
    title: "Business",
    price: "99",
    features: [
      " Full Access",
      "Source Files",
      "Free Appointments",
      "Enhanced Security",
    ],
  },
];
</script>

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
  margin-bottom: 50px;
}
.grid-content {
  border-radius: 4px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px;
  border-radius: 10px;
  margin-bottom: 20px;
}
.grid-content .flex {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.grid-content .icon {
  background: linear-gradient(45deg, #5329c4, #aa65e8) !important;
  height: 80px;
  width: 80px;
  color: #fff;
  font-size: 25px;
  margin-bottom: 15px;
}
.grid-content .flex h3 {
  background: -webkit-linear-gradient(45deg, #5329c4, #aa65e8);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 23px;
}
.grid-content .flex p {
  font-weight: bold;
  font-size: 20px;
}
.grid-content .flex span {
  font-size: 35px;
  padding-bottom: 10px;
}
.grid-content .flex div {
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  width: 100%;
  padding-top: 20px;
}
.features {
  padding: 0 1.5rem !important;
}
.features h5 {
  font-size: 18px;
  margin: 0;
  margin-top: 20px;
}
.list {
  display: flex;
  align-items: center;
  color: #8492a6;
}
.list .features-btn {
  width: 20px;
  height: 20px;
  margin-right: 10px;
}
</style>
