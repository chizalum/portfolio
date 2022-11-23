<template>
  <div>
    <div class="last-layer">
      <p class="services">SERVICES</p>
      <P class="do">What I do for you</P>
      <div class="duties-container">
        <div class="duties">
        </div>
        <div class="duties1">
        </div>
        <div class="duties2">
        </div>
        <div class="duties3">
        </div>
      </div>
    </div>
    <div class="third-layer">
      <div class="name-from">
        <p class="name-col">
          Motivated by the Desire to achieve<span class="span"> Success </span>
        </p>
        <p class="from-col">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Explicabo
          libero accusamus ipsam hic odit qui sunt suscipit? Veniam corrupti
          dicta alias, necessitatibus aspernatur ad repellendus, labore minima
          eos earum natus.
        </p>
      </div>
      <div class="skill-col">
        <div class="languages-txt">
          <p class="specifics-txt">HTML:</p>
          <p class="specifics-txt">CSS:</p>
          <p class="specifics-txt">JavaScript:</p>
          <p class="specifics-txt">VUE:</p>
          <p class="specifics-txt">NUXT:</p>
        </div>
        <div class="percentages">
          <p class="perc-txt">99%</p>
          <p class="perc-txt">99%</p>
          <p class="perc-txt">80%</p>
          <p class="perc-txt">95%</p>
          <p class="perc-txt">90%</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "projects",
};
</script>

<style scoped>
.third-layer {
  margin: 57px 0 0 0;
  background: rgb(235, 226, 226);
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.name-from {
  margin: 0 0 0 30px;
  display: flex;
  flex-direction: column;
  width: 60%;
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

.skill-col {
  display: flex;
  flex-direction: row;
  justify-content: left;
  align-items: flex-start;
  width: 40%;
}

.languages-txt {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 26px;
  margin: 0 160px 0 100px;
}

.percentages{
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 27px;
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
  height: 480px;
  background: url("~/assets/xyz.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 70px 50px;
}

.duties1 {
  width: 450px;
  height: 480px;
  background: url("~/assets/robin-1.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 70px 50px;
}

.duties2 {
  width: 450px;
  height: 480px;
  background: url("~/assets/robin-2.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 70px 50px;
}

.duties3 {
  width: 450px;
  height: 480px;
  background: url("~/assets/robin-3.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 70px 50px;
}

.duties-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin: 0 auto 0 auto;
  height: auto;
  width: 80%;
}

.icons {
  width: 35px;
  height: 35px;
  margin: 30px 0 0 30px;
}

.web {
  margin: 20px 0 0 30px;
}

.lorem {
  margin: 20px 0 0 30px;
}


</style>