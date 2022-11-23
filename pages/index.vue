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
          <button class="btn-1">Hire Me</button>
          <button class="btn-2">Portfolio</button>
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
          <button class="btn-3">View CV</button>
        </a>
      </div>
    </div>
    <div class="last-layer">
      <p class="services">SERVICES</p>
      <P class="do">What I do for you</P>
      <div class="duties-container">
        <div class="duties">
          <img src="app.svg" class="icons" />
          <p class="web">Web Applications</p>
          <p class="lorem">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ut nobis
            porro molestias dolorum sunt eius odio numquam delectus fugit? Odio,
            id cum! Ab quisquam quo sapiente molestiae consequuntur libero
            nobis.
          </p>
        </div>
        <div class="duties">
          <img src="email-icon.svg" class="icons" />
          <p class="web">Email Templates</p>
          <p class="lorem">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ut nobis
            porro molestias dolorum sunt eius odio numquam delectus fugit? Odio,
            id cum! Ab quisquam quo sapiente molestiae consequuntur libero
            nobis.
          </p>
        </div>
        <div class="duties">
          <img src="dev.svg" class="icons" />
          <p class="web">Static Web Pages</p>
          <p class="lorem">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ut nobis
            porro molestias dolorum sunt eius odio numquam delectus fugit? Odio,
            id cum! Ab quisquam quo sapiente molestiae consequuntur libero
            nobis.
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

.btn-3 {
  width: 160px;
  height: 50px;
  border-radius: 12px;
  background: #c8d8e4;
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  cursor: pointer;
  margin: 25px 0 0 25px;
}

.last-layer {
  display: flex;
  flex-direction: column;
  background: whitesmoke;
  height: auto;
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
  background: #703f37;
  margin: 70px 50px;
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
  color: #9c8321;
}

.lorem {
  margin: 20px 0 0 30px;
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
}
</style>
