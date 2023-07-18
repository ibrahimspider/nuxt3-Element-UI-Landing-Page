<template>
  <section>
    <div class="container">
      <div class="header">
        <h3>
          Check out our latest <br />
          news & articles
        </h3>
        <p>
          This is just a simple text made for this unique and awesome template,
          you can replace it with any text.
        </p>
      </div>
      <el-row :gutter="20">
        <el-col :xs="24" :sm="12" :md="8" v-for="post in news">
          <el-card class="box">
            <img :src="post.img" class="image" />
            <div style="padding: 14px">
              <a href="" class="title">{{ post.title }}</a>
              <p class="text-muted">
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </p>
              <a href="" class="btn">Read More</a>
            </div>
          </el-card>
        </el-col>
      </el-row>
    </div>
  </section>
</template>

<script setup>
const news = [
  {
    img: "/img/blog-1.jpg",
    title: "Creativity is nothing but a mind set free",
  },
  {
    img: "/img/blog-2.jpg",
    title: "Simplicity is the ultimate sophistication",
  },
  {
    img: "/img/blog-3.jpg",
    title: "People ignore designs that ignore people",
  },
];
</script>
<style scoped>
section {
  padding: 70px 0;
  background: #f2f6fa;
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

.image {
  width: 100%;
  display: block;
}
.title {
  color: #24272c !important;
  font-size: 20px !important;
  text-decoration: none;
  font-weight: bold;
  line-height: 1.5;
  transition: 300ms all ease-in-out;
}
.title:hover {
  background: -webkit-linear-gradient(45deg, #5329c4, #aa65e8);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.text-muted {
  color: #8492a6 !important;
  line-height: 1.6;
}
.btn {
  line-height: 1.6;
  text-decoration: none;
  color: #24272c;
  position: relative;
  transition: 300ms all ease-in-out;
}
.btn:hover {
  background: -webkit-linear-gradient(45deg, #5329c4, #aa65e8);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.box {
  margin-bottom: 20px;
}
</style>
