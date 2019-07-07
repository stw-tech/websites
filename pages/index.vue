<template>
  <div>
    <div class="section section-top clear-filter">
      <div class="page-header-image" />
      <div class="container">
        <div>
          <logo />
          <h1 class="title">
            T-Tech
          </h1>
          <h2 class="subtitle">
            Fast, Customize Website Solution for Startups.
          </h2>
        </div>
      </div>
    </div>
    <div class="section section-ins section-about">
      <div class="container">
        <div>
          <h1 class="title">
            服務介紹
          </h1>
          <h2 class="subtitle">
            快速建立新創形象頁面
          </h2>
          <p>詳細內容</p>
        </div>
      </div>
    </div>
    <div class="section section-ins section-team">
      <div class="container">
        <div>
          <h1 class="title">
            團隊簡介
          </h1>
          <h2 class="subtitle">
            專業人士，提供專業服務
          </h2>
          <p>人物介紹</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.page-header-image {
  background-image: url('/img/header.jpg');
  position: absolute;
  background-size: cover;
  background-position: 80%;
  background-repeat: no-repeat;
  width: 100%;
  height: 100%;
  z-index: -1;
}

.clear-filter {
  background: linear-gradient(
    0deg,
    rgba(3, 224, 150, 0.253),
    rgba(19, 11, 10, 0.9)
  );
}

.img-blur {
  -webkit-filter: blur(5px);
  -moz-filter: blur(5px);
  -o-filter: blur(5px);
  -ms-filter: blur(5px);
  filter: blur(5px);
}

.section {
  position: relative;
}

.section-about {
  background: #ccc;
}

.section-team {
  background: #eee;
}

.container {
  padding: 70px 0;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.section-top .title {
  color: #f4f9ff;
}

.section-top .subtitle {
  color: #d3d8e0;
}
.section-ins .title {
  font-size: 56px;
  color: #35495e;
  letter-spacing: 1px;
}

.section-ins .subtitle {
  font-size: 30px;
  color: #526488;
  word-spacing: 5px;
  padding-top: 15px;
}

.links {
  padding-top: 15px;
}
</style>
