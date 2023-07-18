<template>
  <section>
    <div class="container">
      <div class="text-center">
        <h2>Subscribe our Newsletter</h2>
        <p>
          This is just a simple text made for this unique and awesome template,
          you can replace it with any text.
        </p>
      </div>
      <div class="box">
        <input type="email" placeholder="Your Email Id" />
        <button>Subscribe Now</button>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
section {
  background: linear-gradient(45deg, #5329c4, #aa65e8);
  padding: 100px 0;
}
.text-center {
  text-align: center;
}
h2 {
  letter-spacing: 0.5px;
  font-size: 31px;
  color: #fff;
}
p {
  margin: auto;
  max-width: 600px;
  font-size: 18px;
  color: rgba(255, 255, 255, 0.5);
  margin-bottom: 50px;
}
.box {
  position: relative;
  text-align: center;
  max-width: 550px;
  margin: auto;
}
.box input {
  padding: 12px 20px;
  width: 100%;
  color: #24272c;
  border: none;
  outline: none;
  padding-right: 160px;
  padding-left: 30px;
  background-color: rgba(255, 255, 255, 0.8);
  height: 50px;
  border-radius: 50rem;
}
.box button {
  position: absolute;
  top: 2px;
  right: 3px;
  outline: none !important;
  border-radius: 30px;
  padding: 15px 20px;
  color: #fff;
  background: linear-gradient(45deg, #5329c4, #aa65e8);
  border: none;
  cursor: pointer;
}
</style>
