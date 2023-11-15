<template>
  <div class="full-screen">
    <section class="top-shelf">
      <div class="intro">
        <div class="me">
          <p class="hello">Hey there,</p>
          <h1 class="chizalum">
            <span class="i-am">I'm </span>Chizalum Joshua
          </h1>
          <div class="content-box">
            <h2 class="box title">Developer</h2>
            <h2 class="box title1">Engineer</h2>
            <h2 class="box title2">Freelancer</h2>
          </div>
          <p class="as">
            As a software engineer, I have a passion for creating amazing
            digital experiences. I'm dedicated to making web applications that
            are both aesthetically pleasing and functional.
          </p>
        </div>
        <div class="buttons">
          <a href="mailto:joshuaegbuonu@gmail.com" target="blank">
            <button class="btn-1">Contact Me</button></a
          >
          <a
            href="https://docs.google.com/document/d/143fc9sRif58tH5U_LwdI_0OIikm5VgmlLWYEOHKWVAo/edit?usp=sharing"
            target="blank"
          >
            <button class="btn-2">Resume</button></a
          >
        </div>
      </div>
    </section>
    <section class="about-layer">
      <div class="central-div">
        <p class="moi">About Me</p>
        <hr class="horizontal" />
        <div class="about-flex">
          <div class="grid-item">
            <p class="desc">
              "Hi! my name is Joshua and I have a passion for developing user
              interfaces that are simple to use and visually appealing. I am
              dedicated to developing aesthetically pleasing and responsive
              online apps that serve user demands
            </p>
          </div>
          <div class="grid-item">
            <img src="about-pic.jpeg" class="profile-pic" alt="profile-pic" />
          </div>
        </div>
        <div class="about-flex1">
          <div class="grid-item">
            <p class="desc">
              I specialize in developing intuitive user interfaces that enhance
              user experience and engagement. I'm always looking for new methods
              to develop my abilities and provide creative solutions."
            </p>
          </div>
          <div class="grid-item">
            <p class="desc">I'm proficient in :</p>
            <div class="second-grid">
              <div class="frame">HTML</div>
              <div class="frame">CSS</div>
              <div class="frame">JavaScript</div>
              <div class="frame">Wordpress</div>
              <div class="frame">Vue.js</div>
              <div class="frame">Nuxt.js</div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="last-layer">
      <div class="central-div">
        <p class="moi">Work experience</p>
        <hr class="horizontal" />
        <div class="site-settings">
          <div class="site">
            <button
              class="experience1"
              :class="{ rotate: showDetails, highlight: highDetails }"
              @click="writeDetails"
              @mouseover="startHover()"
              @mouseleave="stopHover()"
            >
              <p class="org" :class="{ bold: showDetails }">Acumen Digital</p>
            </button>

            <button
              class="experience"
              :class="{ rotate: showDetails1, highlight: highDetails1 }"
              @click="writeDetails1"
              @mouseover="startHover1()"
              @mouseleave="stopHover1()"
            >
              <p class="org" :class="{ bold: showDetails1 }">
                Nigeria Security Printing and Minting
              </p>
            </button>
            <button
              class="experience"
              :class="{ rotate: showDetails2, highlight: highDetails2 }"
              @click="writeDetails2"
              @mouseover="startHover2()"
              @mouseleave="stopHover2()"
            >
              <p class="org" :class="{ bold: showDetails2 }">Nasco</p>
            </button>
          </div>
          <hr class="ruling" />
          <Acumen
            v-if="showAcumen"
            class="insert"
            :class="{ bring: showAcumen }"
          ></Acumen>
          <Nasco
            v-if="showNasco"
            class="insert"
            :class="{ bring: showNasco }"
          ></Nasco>
          <Nspm
            v-if="showNspm"
            class="insert"
            :class="{ bring: showNspm }"
          ></Nspm>
        </div>
      </div>
    </section>
    <section class="work-load">
      <div class="central-div">
        <p class="moi">Projects</p>
        <hr class="horizontal" />
        <div class="wraith">
          <p class="projects-text">Welcome to my Projects Section</p>
          <p class="projects-intro">
            Explore my work, one project at a time. Each project is like a
            puzzle piece in my journey as a software engineer and technology
            enthusiast. Click on a project below to view the demo site.
          </p>
        </div>
        <div class="row-div">
          <a
            class="project"
            href="https://master--keen-custard-aaed08.netlify.app/"
            target="blank"
          >
            <div class="blur"></div>
            <div class="banner">
              <button class="writings">
                XYZ Logistics<br /><span class="admin">Admin Dashboard</span>
              </button>
            </div>
          </a>

          <a
            class="project-two"
            href="https://master--lambent-cannoli-619c43.netlify.app/"
            target="blank"
          >
            <div class="blur-two"></div>
            <div class="banner-two">
              <button class="writings-two">
                Yohagi Store<br /><span class="admin-two">Online Store</span>
              </button>
            </div>
          </a>


          <a
            class="project-three"
            href="https://master--chic-maamoul-84c7dd.netlify.app/"
            target="blank"
          >
            <div class="blur-three"></div>
            <div class="banner-three">
              <button class="writings-three">
                Robin App<br /><span class="admin-three">Landing Page</span>
              </button>
            </div>
          </a>


        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      showDetails: true,
      showDetails1: false,
      showDetails2: false,
      highDetails: false,
      highDetails1: false,
      highDetails2: false,
      showAcumen: true,
      showNasco: false,
      showNspm: false,
    };
  },

  methods: {
    writeDetails() {
      this.showDetails = true;
      this.showDetails1 = false;
      this.showDetails2 = false;
      this.highDetails = false;
      this.showAcumen = true;
      this.showNspm = false;
      this.showNasco = false;
    },

    writeDetails1() {
      this.showDetails1 = true;
      this.showDetails = false;
      this.showDetails2 = false;
      this.highDetails1 = false;
      this.showNspm = true;
      this.showAcumen = false;
      this.showNasco = false;
    },

    writeDetails2() {
      this.showDetails2 = true;
      this.showDetails1 = false;
      this.showDetails = false;
      this.highDetails2 = false;
      this.showNasco = true;
      this.showNspm = false;
      this.showAcumen = false;
    },

    startHover() {
      if (this.showDetails == false) {
        this.highDetails = true;
      }
    },

    startHover1() {
      if (this.showDetails1 == false) {
        this.highDetails1 = true;
      }
    },

    startHover2() {
      if (this.showDetails2 == false) {
        this.highDetails2 = true;
      }
    },

    stopHover() {
      this.highDetails = false;
    },

    stopHover1() {
      this.highDetails1 = false;
    },

    stopHover2() {
      this.highDetails2 = false;
    },
  },
};
</script>

<style scoped>
.full-screen {
  scroll-snap-type: y mandatory;
  overflow-y: scroll;
  height: 100vh;
}

.top-shelf {
  width: 100%;
  margin: 0 auto 0 auto;
  scroll-snap-align: start;
  height: auto;
  padding: 115px 0 115px 0;
}

.about-layer {
  width: 100%;
  margin: 0 auto 0 auto;
  scroll-snap-align: start;
  height: auto;
  padding: 115px 0 115px 0;
}

.central-div {
  width: 649px;
  margin: 0 auto 0 auto;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  height: 100%;
  padding: 0 0 0 0;
}

.profile-pic {
  height: 240px;
  width: 280px;
  border-radius: 25%;
}

.intro {
  width: 649px;
  margin: 0 auto 0 auto;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  height: 100%;
  padding: 0 0 0 0;
}

.me {
  display: flex;
  flex-direction: column;
  width: 100%;
  font-size: 27px;
}

.hello {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
  margin: 0 0 0 0;
  color: rgb(172, 138, 138);
}

.moi {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
  margin: 0 0 0 0;
  color: #fff5ee;
}

.horizontal {
  width: 100%;
  border: 1px solid #09212e;
}

.i-am {
  font-family: "Aboreto-Regular";
  font-weight: 400;
  font-size: 46px;
  color: rgb(195, 190, 190);
}

.content-box {
  margin: 90px auto 70px auto;
  width: 100%;
  position: relative;
}

.about-flex {
  display: flex;
  width: 100%;
  height: auto;
  flex-direction: row;
  align-items: center;
  margin: 32px auto 0 auto;
}

.about-flex1 {
  display: flex;
  width: 100%;
  height: auto;
  flex-direction: row;
  margin: 64px auto 0 auto;
}

.second-grid {
  display: grid;
  width: 280px;
  height: 100%;
  grid-template-columns: 50% 50%;
  grid-template-rows: 33% 33% 33%;
  align-items: end;
  margin: auto 0 0 0;
}

.grid-item {
  width: 50%;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.box {
  font-size: 46px;
  font-weight: 200;
  opacity: 0;
  position: absolute;
  margin: auto;
  width: 100%;
  text-align: center;
  z-index: 999999;
  color: rgb(195, 190, 190);
  font-family: "Raleway-VariableFont_wght";
}

.title {
  animation: ani1 15s infinite;
}

.title1 {
  animation: ani2 15s infinite;
}

.title2 {
  animation: ani3 15s infinite;
}

.as {
  font-family: "RobotoMono-VariableFont_wght";
  font-weight: 400;
  font-size: 16px;
  color: #d8b5b5;
  width: 649px;
  text-align: justify;
}

.desc {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 16px;
  color: #d8b5b5;
  text-align: justify;
  width: 280px;
  margin: 0;
}

.frame {
  color: rgb(195, 190, 190);
  font-family: "Raleway-VariableFont_wght";
  font-size: 16px;
  text-align: justify;
  margin: 0;
}

.frame:nth-child(2) {
  justify-self: end;
}

.frame:nth-child(4) {
  justify-self: end;
}

.frame:nth-child(6) {
  justify-self: end;
}

@keyframes ani1 {
  0% {
    opacity: 0;
  }
  17% {
    opacity: 1;
  }
  33% {
    opacity: 0;
  }
}

@keyframes ani2 {
  33% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  66% {
    opacity: 0;
  }
}

@keyframes ani3 {
  66% {
    opacity: 0;
  }
  83% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}

@keyframes cursor {
  0% {
    border-color: transparent;
  }
  17% {
    border-color: grey;
  }
  33% {
    border-color: transparent;
  }

  50% {
    border-color: grey;
  }
  66% {
    border-color: transparent;
  }

  83% {
    border-color: grey;
  }
  100% {
    border-color: transparent;
  }
}

@keyframes typing {
  0% {
    width: 0%;
  }
  50% {
    width: 50%;
  }
  100% {
    width: 100%;
  }
}

.chizalum {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 800;
  font-size: 59px;
  color: #fff5ee;
  margin: 70px 0 0 0;
  border-right: 5px solid transparent;
  white-space: nowrap;
  overflow: hidden;
  animation: typing 4s steps(19, end), cursor 4s step-end 1 ;
  width: 600px;
}

.buttons {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin: 70px 0 0 0;
}

.btn-1 {
  width: 160px;
  height: 50px;
  border-radius: 12px;
  background: rgb(183, 196, 178);
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  color: rgb(68, 149, 68);
  cursor: pointer;
}

.btn-1:hover {
  background: rgb(227, 243, 221);
}

.btn-2:hover {
  background: rgb(227, 243, 221);
}
.btn-2 {
  width: 160px;
  height: 50px;
  margin: 0 0 0 20px;
  border-radius: 12px;
  background: rgb(183, 196, 178);
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  color: rgb(68, 149, 68);
  cursor: pointer;
}

.last-layer {
  width: 100%;
  margin: 0 auto 0 auto;
  scroll-snap-align: start;
  height: auto;
  padding: 115px 0 115px 0;
}

.site-settings {
  width: 100%;
  height: auto;
  padding: 0;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}

.site {
  height: 480px;
  width: 36%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
  margin: 30px 0 0 0;
}

.ruling {
  border: 2px solid #d8b5b5;
  margin: 30px auto 0 auto;
}

.experience {
  margin: 25px 0 0 0;
  width: 90%;
  height: auto;
  cursor: pointer;
  border-radius: 12px;
  border: none;
  background: #ebe9e9;
}

.experience1 {
  margin: 0 0 0 0;
  width: 90%;
  height: auto;
  border-radius: 12px;
  border: none;
  cursor: pointer;
  background: #ebe9e9;
}

.rotate {
  border-radius: 12px;
  background: rgb(183, 196, 178);
  border: none;
  cursor: pointer;
  animation: clicked 0.5s ease-in-out forwards;
}

@keyframes clicked {
  0% {
    transform: scaleX(97%);
  }
  25% {
    transform: scaleX(100%);
  }
  50% {
    transform: scaleX(103%);
  }
  100% {
    transform: scaleX(106%);
  }
}


.bring {
  animation: ship 0.8s ease-in forwards;
}

@keyframes ship {
  0% {
    transform: translateY(-12%);
    opacity: 0.1;
  }
  25% {
    transform: translateY(-9%);
    opacity: 0.3;
  }
  50% {
    transform: translateY(-6%);
    opacity: 0.5;
  }
  75% {
    transform: translateY(-3%);
    opacity: 0.7;
  }
  100% {
    transform: translateY(0%);
    opacity: 1;
  }
}

.highlight {
  background: rgb(227, 243, 221);
}

.org {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 800;
  font-size: 12px;
  color: #767872;
}

.bold {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 800;
  font-size: 14px;
  color: rgb(68, 149, 68);
}

#prince {
  margin: 20px 25px 0 30px;
  font-family: "Aboreto-Regular";
  font-weight: 3;
  font-size: 13px;
  font-weight: 200;
}

.work-load {
  width: 100%;
  margin: 0 auto 0 auto;
  scroll-snap-align: start;
  height: auto;
  padding: 112px 0 112px 0;
}

.row-div {
  width: 100%;
  height: 640px;
  margin: 30px 0 0 0;
  display: flex;
  flex-direction: column;
  overflow-x: auto;
}

.project {
  min-width: 350px;
  min-height: 400px;
  margin: 30px auto 0 auto;
  border-radius: 16px;
  border: none;
  cursor: pointer;
  text-decoration: none;
  position: relative;
}

.blur {
  background: url("~/assets/xyz.png");
  background-position: center;
  background-size: 350px 400px;
  background-repeat: no-repeat;
  width: 100%;
  height: 100%;
  transition: all 1s;
  border-radius: 10px;
}

.banner {
  width: 100%;
  min-height: 50px;
  background: none;
  margin: 0;
  opacity: 0;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  transition: all 1s;
  overflow: hidden;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
}

.project:hover .banner {
  opacity: 1;
}

.project:hover .blur {
  opacity: 0.3;
  filter: blur(6px);
}



.project-two {
  min-width: 350px;
  min-height: 400px;
  margin: 30px auto 0 auto;
  border-radius: 16px;
  border: none;
  cursor: pointer;
  text-decoration: none;
  position: relative;
}

.blur-two {
  background: url("~/assets/yohagi.png");
  background-position: center;
  background-size: 350px 400px;
  background-repeat: no-repeat;
  width: 100%;
  height: 100%;
  transition: all 1s;
  border-radius: 10px;
}

.banner-two {
  width: 100%;
  min-height: 50px;
  background: none;
  margin: 0;
  opacity: 0;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  transition: all 1s;
  overflow: hidden;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
}

.project-two:hover .banner-two {
  opacity: 1;
}

.project-two:hover .blur-two {
  opacity: 0.3;
  filter: blur(6px);
}


.project-three {
  min-width: 350px;
  min-height: 400px;
  margin: 30px auto 0 auto;
  border-radius: 16px;
  border: none;
  cursor: pointer;
  text-decoration: none;
  position: relative;
}

.blur-three {
  background: url("~/assets/robin-1.png");
  background-position: center;
  background-size: 350px 400px;
  background-repeat: no-repeat;
  width: 100%;
  height: 100%;
  transition: all 1s;
  border-radius: 10px;
}

.banner-three {
  width: 100%;
  min-height: 50px;
  background: none;
  margin: 0;
  opacity: 0;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  transition: all 1s;
  overflow: hidden;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
}

.project-three:hover .banner-three {
  opacity: 1;
}

.project-three:hover .blur-three {
  opacity: 0.3;
  filter: blur(6px);
}

.writings {
  width: 160px;
  height: 50px;
  border-radius: 12px;
  background: #01151f;
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  color: rgb(68, 149, 68);
  cursor: pointer;
  font-weight: 600;
  text-decoration: none;
}

.writings-two {
  width: 160px;
  height: 50px;
  border-radius: 12px;
  background: #01151f;
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  color: rgb(68, 149, 68);
  cursor: pointer;
  font-weight: 600;
  text-decoration: none;
}

.writings-three {
  width: 160px;
  height: 50px;
  border-radius: 12px;
  background: #01151f;
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  color: rgb(68, 149, 68);
  cursor: pointer;
  font-weight: 600;
  text-decoration: none;
}

.admin {
  font-size: 16px;
  color: rgb(68, 149, 68);
  font-weight: 400;
}


.admin-two{
  font-size: 16px;
  color: rgb(68, 149, 68);
  font-weight: 400;
}

.admin-three {
  font-size: 16px;
  color: rgb(68, 149, 68);
  font-weight: 400;
}
.wraith {
  margin: 0 auto 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
  width: 100%;
  height: auto;
}

.projects-text {
  font-family: "Raleway-VariableFont_wght";
  color: #fff5ee;
  font-weight: 400;
  margin: 10px 0 10px 0;
  font-size: 20px;
}

.projects-intro {
  color: #d8b5b5;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 200;
  font-size: 16px;
  margin: 0;
}

@media (max-width: 685px) {
  .central-div {
    width: 96%;
    margin: 0 auto 0 auto;
  }

  .intro {
    width: 96%;
    margin: 0 auto 0 auto;
  }
  .hello {
    font-size: 17px;
  }

  .chizalum {
    font-size: 30px;
    width: 300px;
  }

  .i-am {
    font-size: 26px;
  }

  .box {
    font-size: 26px;
  }
  .as {
    width: 96%;
    margin: 0 auto 0 auto;
  }

  .profile-pic{
    height: 150px;
    width: 95%;
  }

  .desc{
    width: 95%;
    text-align: justify;
    font-size: 12px;
  }

  .frame{
    font-size: 12px;
  }

  .as{
    font-size: 13px;
  }

  .second-grid{
    width: 95%;
  }

  .btn-1{
    width: 140px;
    font-size: 16px;
  }

  .btn-2{
    width: 140px;
    font-size: 16px;
  }

  .moi{
    font-size: 22px;
  }

  .org{
    font-size: 8px;
  }

  .bold{
    font-size: 10px;
  }


  .projects-text{
    font-size: 18px;
  }

  .projects-intro{
    font-size: 14px;
  }

  .project{
    min-width: 300px;
    min-height: 370px;
  }

  .project-two{
    min-width: 300px;
    min-height: 370px;
  }

  .project-three{
    min-width: 300px;
    min-height: 370px;
  }

  .blur{
    background-size: 300px 370px;
  }

  .blur-two{
    background-size: 300px 370px;
  }

  .blur-three{
    background-size: 300px 370px;
  }
}
</style>
