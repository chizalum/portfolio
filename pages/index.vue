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
            href="https://drive.google.com/file/d/1ybXWFFsz5Ituwu8XqPlaNIiJzLC62rho/view?usp=sharing"
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
        <div class="about-grid">
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
              <p class="frame">HTML</p>
              <p class="frame">CSS</p>
              <p class="frame">JavaScript</p>
              <p class="frame">Wordpress</p>
              <p class="frame">Vue</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="last-layer">
      <p class="services">SERVICES</p>
      <P class="do">What I do for you</P>
      <div class="duties-container">
        <div class="duties">
          <img src="ig-profile.svg" class="icons" />
          <p class="web">Web Applications</p>
          <p class="lorem">
            Create <span class="span">WEB APPLICATIONS</span> for your business.
          </p>
          <P class="description"
            >Use these dynamic websites to interact with customers, sell goods
            and services, pass information and recieve information. These could
            include online forms, shopping carts, word processors and file
            conversion websites.</P
          >
        </div>
        <div class="duties">
          <img src="blue-mail.svg" class="icons" />
          <p class="web">Email Templates</p>
          <p class="lorem">
            Create beautiful <span class="span">EMAIL TEMPLATES</span> for your
            business.
          </p>
          <p class="description">
            Send html mails to a mail list and advertise your service or
            business.
          </p>
        </div>
        <div class="duties">
          <img src="red-site.svg" class="icons" />
          <p class="web">Static Web Pages</p>
          <p class="lorem">
            Create <span class="span"> STATIC WEBSITES</span> for your business.
          </p>
          <p class="description">
            These are small websites that are limited in content, and don't
            require frequent updates. This includes brochure websites, one-off
            landing pages, and other informational or read-only sites.
          </p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import { onMounted, onUnmounted } from "vue";
export default {
  name: "IndexPage",
  data: () => {},
};
</script>

<style scoped>
.full-screen {
  scroll-snap-type: y mandatory;
  overflow-y: scroll;
  height: 100vh;
}

.top-shelf {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin: 0 auto 0 auto;
  padding-top: 115px;
  align-items: center;
  scroll-snap-align: start;
  height: auto;
}

.about-layer {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin: 115px auto 0 auto;
  align-items: center;
  scroll-snap-align: start;
  height: auto;
  padding-top: 115px;
}

.central-div {
  width: 649px;
  margin: 0 auto 0 auto;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.profile-pic {
  height: 240px;
  width: 280px;
  border-radius: 25%;
}

.intro {
  display: flex;
  flex-direction: column;
  margin: 0 0 0 0;
  display: inline-block;
  width: fit-content;
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
  color: rgb(172, 138, 138);
}

.horizontal {
  width: 100%;
  color: rgb(195, 190, 190);
  background: rgb(195, 190, 190);
}

.apost {
  color: rgb(195, 190, 190);
  font-size: 40px;
  font-family: "Aboreto-Regular";
}

.apost2 {
  color: rgb(195, 190, 190);
  font-size: 40px;
  justify-self: flex-end;
  font-family: "Aboreto-Regular";
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

.about-grid {
  display: grid;
  width: 649px;
  height: max-content;
  grid-template-columns: 50% 50%;
  grid-template-rows: 240px 240px;
  justify-content: space-evenly;
  align-items: flex-start;
  grid-row: 30px;
}

.second-grid {
  display: grid;
  width: 280px;
  height: 100%;
  grid-template-columns: 50% 50%;
  grid-template-rows: 33.3% 33.3% 33.3%;
  grid-row: 30px;
  justify-content: space-between;
  margin: auto 0 0 0;
  background: orange;
}

.grid-item {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
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
  font-family: "RobotoMono-VariableFont_wght";
  font-weight: 400;
  font-size: 16px;
  color: #d8b5b5;
  text-align: justify;
  width: 280px;
  margin: 0;
}

.frame {
  font-family: "Raleway-VariableFont_wght";
  color: #fcf5e5;
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
    border-color: white;
  }
  17% {
    border-color: transparent;
  }
  33% {
    border-color: white;
  }

  0% {
    border-color: transparent;
  }
  50% {
    border-color: white;
  }
  66% {
    border-color: transparent;
  }

  83% {
    border-color: white;
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
  border-right: 5px solid white;
  white-space: nowrap;
  overflow: hidden;
  animation: typing 4s steps(19, end), cursor 6s step-end infinite;
  width: 649px;
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
  display: flex;
  flex-direction: column;
  height: auto;
  padding: 0 0 70px 0;
  scroll-snap-align: start;
  background: wheat;
}

.services {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 0;
  font-size: 22px;
  margin: 70px auto 0 auto;
  text-align: center;
}

.do {
  font-family: "Aboreto-Regular";
  font-weight: 800;
  font-size: 46px;
  color: rgb(63, 50, 50);
  text-align: center;
  margin: 70px auto 0 auto;
}

.duties {
  width: 450px;
  height: 280px;
  background: linear-gradient(180deg, #f5f5f5, #e9ddd4);
  backdrop-filter: saturate(180%) blur(10px);
  margin: 70px 50px;
}

@supports (-webkit-backdrop-filter: none) or (backdrop-filter: none) {
  .duties {
    -webkit-backdrop-filter: blur(10px);
    backdrop-filter: blur(10px);
  }
}

.duties-container {
  display: flex;
  flex-direction: row;
}

.icons {
  width: 35px;
  height: 35px;
  margin: 30px 0 0 30px;
}

.web {
  margin: 20px 0 0 30px;
  color: #685612;
  text-decoration: solid;
  font-size: 20px;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 900;
}

.span {
  color: #685612;
  text-decoration: solid;
  font-size: 15px;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 600;
}

.lorem {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 40;
  font-size: 14px;
  margin: 20px 25px 0 30px;
  font-weight: 300;
}

.description {
  margin: 20px 25px 0 30px;
  font-family: "Aboreto-Regular";
  font-weight: 3;
  font-size: 13px;
  font-weight: 200;
}

@media (max-width: 1309px) {
  .second-layer {
    margin: 90px 0 0 0;
    background: #e1eedd;
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .duties-container {
    display: flex;
    flex-direction: column;
  }

  .duties {
    width: 450px;
    height: 280px;
    background: rgb(235, 226, 226);
    margin: 20px auto 0 auto;
  }

  .top-shelf {
    display: flex;
    flex-direction: column;
    width: 100%;
    margin: 115px auto 0 auto;
  }

  .profile-pic {
    margin-left: 8px;
  }

  .intro {
    margin-left: 8px;
  }

  .personal-logo {
    height: fit-content;
    width: 80%;
  }

  .do {
    font-family: "Aboreto-Regular";
    font-weight: 800;
    font-size: 36px;
    color: rgb(63, 50, 50);
    text-align: center;
    margin: 70px auto 0 auto;
  }
}

@media (max-width: 450px) {
  .duties {
    width: 95%;
    height: 320px;
    background: rgb(235, 226, 226);
    margin: 20px auto 0 auto;
  }
}
</style>
