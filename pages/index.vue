<template>
  <div>
    <div class="section section-top clear-filter">
      <div class="page-header-image" />
      <div class="container">
        <div>
          <logo />
          <h1 class="title">
            Remoneer
          </h1>
          <h2 class="subtitle">
            Fast, Stable, Scalable IT Solution.
          </h2>
        </div>
      </div>
    </div>
    <div id="product" class="section section-ins section-product">
      <div class="container">
        <div>
          <h1 class="title">
            Product
          </h1>
          <h2 class="subtitle">
            整合式的 IT 解決方案
          </h2>
          <div>
            <b-container fluid>
              <b-row v-scroll-reveal.reset="{ duration: 800 }" align-h="center">
                <b-col md="2">
                  <b-img
                    src="/svg/computer-1.svg"
                    fluid
                    alt="Responsive image"
                  />
                  <h4 class="mt-4">
                    Web Service
                  </h4>
                </b-col>
                <b-col md="2">
                  <b-img
                    src="/svg/documents.svg"
                    fluid
                    alt="Responsive image"
                  />
                  <h4 class="mt-4">
                    E-mail & Office Software
                  </h4>
                </b-col>
                <b-col md="2">
                  <div>
                    <b-img
                      src="/svg/binder.svg"
                      width="1000"
                      fluid
                      alt="Responsive image"
                    />
                    <h4 class="mt-4">
                      Storage Space
                    </h4>
                  </div>
                </b-col>
                <b-col md="2">
                  <b-img src="/svg/list.svg" fluid alt="Responsive image" />
                  <h4 class="mt-4">
                    Project Management
                  </h4>
                </b-col>
                <b-col md="2">
                  <b-img src="/svg/chat.svg" fluid alt="Responsive image" />
                  <h4 class="mt-4">
                    Communication & Consolidation
                  </h4>
                </b-col>
                <b-col md="2">
                  <b-img src="/svg/receipt.svg" fluid alt="Responsive image" />
                  <h4 class="mt-4">
                    Accounting Issue
                  </h4>
                </b-col>
              </b-row>
            </b-container>
          </div>
        </div>
      </div>
    </div>
    <div id="solution" class="section section-ins section-about">
      <div class="container">
        <div>
          <h1 class="title">
            Our Advantage
          </h1>
          <h2 class="subtitle">
            .
          </h2>
          <div
            v-scroll-reveal.reset="{ duration: 800 }"
            class="service-contents"
          >
            <ul class="list-unstyled">
              <b-media
                class="mt-4"
                right-align
                vertical-align="center"
                tag="li"
              >
                <b-img
                  slot="aside"
                  blank-color="#fff"
                  width="200"
                  alt="placeholder"
                  src="/svg/startup.svg"
                />

                <h5 class="mt-0 mb-1 subtitle" style="text-align:right">
                  Fast, Stable, Scalable Construstion.
                </h5>
              </b-media>
              <b-media class="mt-4" vertical-align="center" tag="li">
                <b-img
                  slot="aside"
                  blank-color="#fff"
                  width="200"
                  alt="placeholder"
                  src="/svg/tablet.svg"
                />

                <h5 class="mt-0 mb-1 subtitle">
                  Establish All IT Service You Need.
                </h5>
              </b-media>
              <b-media
                class="mt-4"
                right-align
                vertical-align="center"
                tag="li"
              >
                <b-img
                  slot="aside"
                  blank-color="#fff"
                  width="200"
                  alt="placeholder"
                  src="/svg/meeting.svg"
                />

                <h5 class="mt-0 mb-1 subtitle" style="text-align:right">
                  Consult When You Have Any Problem.
                </h5>
              </b-media>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div id="team" class="section section-ins section-team">
      <div class="container">
        <div>
          <h1 class="title">
            Team
          </h1>
          <div>
            <b-card-group v-scroll-reveal.reset="{ duration: 800 }" deck>
              <b-card
                title="Conrad lan"
                img-src="https://picsum.photos/300/300/?image=41"
                img-alt="Image"
                img-top
              >
                <b-card-text>
                  Info
                </b-card-text>
              </b-card>
            </b-card-group>
          </div>
        </div>
      </div>
    </div>
    <div id="info" class="section section-info">
      <div class="container">
        <div>
          <h1 class="subtitle">
            Info
          </h1>
          <div>
            <p>Remoneer inc.</p>
            <p>service@remoneer.com</p>
            <p>0800-XXX-XXX</p>
          </div>
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
    rgba(128, 127, 121, 0.308)
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
  background: rgba(175, 180, 169, 0.658);
}

.section-team {
  background: #eee;
}

.section-info {
  background: #35495e;
}

.container {
  padding: 70px 0;
  margin: 0 auto;
  min-height: 80vh;
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
  color: #eaf0f8;
  letter-spacing: 1.5px;
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

.section-info .subtitle {
  color: aliceblue;
}

.section-info p {
  color: aliceblue;
}

.links {
  padding-top: 15px;
}

.service-contents {
  text-align: left;
  float: left;
  width: 750px;
}
</style>
