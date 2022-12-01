<template>
  <div class="full-screen">
    <Tutorial />
    <div class="top-shelf">
      <div class="intro">
        <p class="hello">HELLO,</p>
        <h1 class="chizalum">
          <span class="i-am">I'm </span>Chizalum<br />
          Joshua Egbuonu
        </h1>
        <p class="roles">Developer / Engineer / Freelancer</p>
        <div class="buttons">
          <a href="mailto:joshuaegbuonu@gmail.com" target="blank">
            <button class="btn-1">Hire Me</button></a
          >
          <a
            href="https://drive.google.com/file/d/1ybXWFFsz5Ituwu8XqPlaNIiJzLC62rho/view?usp=sharing"
            target="blank"
          >
            <button class="btn-2">Resume</button></a
          >
        </div>
      </div>
      <img src="profile-pic.png" class="profile-pic" alt="profile-pic" />
    </div>
    <div class="second-layer">
      <img src="personal-logo.svg" class="personal-logo" />
      <div class="column-layer">
        <p class="who">WHO AM I?</p>
        <p class="passion">
          I'm <span>Chizalum Joshua Egbuonu,</span> a Front-end Developer.
        </p>
        <p class="tech">
          Hi there! I have been very passionate about technology for as long as
          i can remember. I am currently a front-end developer, speacialised in
          building web applications using Vue.js / Nuxt.js.
        </p>
        <a
          href="https://drive.google.com/file/d/1ybXWFFsz5Ituwu8XqPlaNIiJzLC62rho/view?usp=sharing"
          download
          target="blank"
        >
        </a>
      </div>
    </div>
    <div class="last-layer">
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
            Create beautiful <span class="span">EMAIL TEMPLATES</span> for your business.
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
    </div>
  </div>
</template>
<!--color: rgb(208, 248, 248)-->
<script>
export default {
  name: "IndexPage",
};
</script>

<style scoped>
.top-shelf {
  display: flex;
  flex-direction: row;
  width: 100%;
  margin: 115px auto 0 auto;
  justify-content: center;
}

.profile-pic {
  height: 320px;
  width: 340px;
  border-radius: 40%;
}

.intro {
  display: flex;
  flex-direction: column;
  margin: 0 90px 0 0;
}

.hello {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
  margin: 0 0 0 0;
}

.i-am {
  font-family: "Aboreto-Regular";
  font-weight: 400;
  font-size: 46px;
  color: black;
}

.chizalum {
  font-family: "Aboreto-Regular";
  font-weight: 800;
  font-size: 46px;
  color: rgb(63, 50, 50);
  margin: 70px 0 0 0;
}

.roles {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 26px;
  margin: 55px 0 0 0;
}

.buttons {
  display: flex;
  flex-direction: row;
  margin: 30px 0 0 0;
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

.btn-2 {
  width: 160px;
  height: 50px;
  margin: 0 0 0 20px;
  border-radius: 12px;
  background: rgb(227, 243, 221);
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  color: rgb(68, 149, 68);
  cursor: pointer;
}

.second-layer {
  margin: 90px 0 0 0;
  background: #e1eedd;
  display: flex;
  flex-direction: row;
}

.personal-logo {
  height: fit-content;
  width: fit-content;
}

.column-layer {
  display: flex;
  flex-direction: column;
}

.who {
  font-family: "Aboreto-Regular";
  font-weight: 0;
  font-size: 27px;
  margin: 87px 0 0 25px;
}

.passion {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 46px;
  margin: 65px 0 0 25px;
}

.tech {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
  margin: 25px 0 0 25px;
}


.last-layer {
  display: flex;
  flex-direction: column;
  background: whitesmoke;
  height: auto;
  padding: 0 0 70px 0;
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

.span{
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

.description{
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

  .personal-logo {
    margin: 0 auto 0 auto;
  }

  .top-shelf {
    display: flex;
    flex-direction: column-reverse;
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
