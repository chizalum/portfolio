<template>
  <div>
    <div class="first-layer">
      <p class="about">About Me</p>
    </div>
    <div class="second-layer">
      <img src="about-pic.jpeg" class="personal-logo" />
      <div class="column-layer">
        <p class="engineer">On my way to being a full-stack developer...</p>
        <p class="passion">Having A Passion For Technology</p>
        <p class="tech">
          Hey there! I have been very passionate about technology and it's
          impact in people's lives for as long as i can remember. I dream of
          developing expert software that has significant value in people's
          lives. I am currently a front-end developer, on my way to becoming a
          full-stack developer.
        </p>
      </div>
    </div>
    <div class="pre-third">
      <hr class="horizontal-rule" />
      <div class="third-layer">
        <div class="name-from">
          <p class="name-col">
            <span class="span">Name: </span>Chizalum Joshua Egbuonu
          </p>
          <p class="from-col">
            <span class="span">Email: </span>joshuaegbuonu@gmail.com
          </p>
        </div>
        <div class="name-from1">
          <p class="name-col"><span class="span">Age: </span>22</p>
          <p class="from-col"><span class="span">From: </span>Nigeria</p>
        </div>
      </div>
      <div class="link">
        <a
          href="https://drive.google.com/file/d/1ybXWFFsz5Ituwu8XqPlaNIiJzLC62rho/view?usp=sharing"
          download
          target="blank"
        >
          <button class="btn-3">Download CV</button>
        </a>
      </div>
    </div>
     <div class="last-layer">
      <p class="services">WORK</p>
      <P class="do">My work Experience</P>
      <div class="duties-container">
        <div class="duties">
          <img src="dev.svg" class="icons" />
          <p class="web">Acumen Digital</p>
          <p class="lorem">
            Software engineering intern
          </p>
          <ul>
            <li>User Interface build.</li>
            <li>Bug fixes and optimization.</li>
            <li>Front end web development.</li>
            <li>Built Single Page Applications utilizing RESTFU APIs.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "about",
};
</script>

<style scoped>
.first-layer {
  width: 100%;
  height: 195px;
  background: whitesmoke;
  margin: 57px 0 0 0;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.about {
  font-family: "Aboreto-Regular";
  font-size: 36px;
  font-weight: 900;
  margin: auto auto auto auto;
  text-align: center;
  color: rgb(68, 149, 68);
}

.second-layer {
  margin: 0 0 0 0;
  background: rgb(235, 226, 226);
  display: flex;
  flex-direction: row;
}

.personal-logo {
  height: 500px;
  width: 650px;
}

.column-layer {
  display: flex;
  flex-direction: column;
}

.engineer {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 46px;
  margin: 87px 0 0 18px;
  font-weight: 0;
}

.passion {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
  margin: 65px 0 0 18px;
  font-weight: 1000;
}

.tech {
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
  margin: 25px 0 105px 18px;
}

.pre-third {
  background: rgb(235, 226, 226);
  margin: 0 0 0 0;
}

.third-layer {
  margin: 0 0 0 0;
  background: rgb(235, 226, 226);
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.name-from {
  margin: 0 280px 0 0;
  display: flex;
  flex-direction: column;
}

.name-from1 {
  margin: 0 0 0 0;
  display: flex;
  flex-direction: column;
}

.horizontal-rule {
  margin: 0 auto 65px auto;
  color: rgb(68, 149, 68);
  height: 2px;
  background: rgb(68, 149, 68);
  width: 80%;
  text-align: center;
}

.name-col {
  font-family: "Raleway-VariableFont_wght";
  font-size: 26px;
}

.from-col {
  font-family: "Raleway-VariableFont_wght";
  font-size: 26px;
}

.span {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 26px;
}

.link {
  text-align: center;
}

.btn-3 {
  width: 160px;
  height: 50px;
  border-radius: 12px;
  background: rgb(227, 243, 221);
  border: none;
  font-family: "Raleway-VariableFont_wght";
  font-size: 20px;
  background: rgb(146, 119, 119);
  cursor: pointer;
  margin: 25px auto 65px auto;
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
  background: rgb(235, 226, 226);
  margin: 70px auto 50px auto;
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
  font-family: "Raleway-VariableFont_wght";
  font-weight: 800;
  font-size: 26px;
}

.lorem {
  margin: 20px 0 0 30px;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 20px;
}

.list-items{

}

@media (max-width: 1309px) {
  .second-layer {
    margin: 0 0 0 0;
    background: rgb(235, 226, 226);
    display: flex;
    flex-direction: column;
  }

  .personal-logo {
  height: 500px;
  width: 650px;
  margin: 0 auto 0 auto;
}

.name-from {
  margin: 0 30px 0 0;
  display: flex;
  flex-direction: column;
}
}
</style>