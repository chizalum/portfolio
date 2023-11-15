<template>
  <div class="light">
    <div class="light-header">
      <div class="wraith-point">
        <P class="wraith"
          >Acumen Digital <span class="span"><br>Software Engineer</span></P
        >
        <p class="break">2022</p>
      </div>
      <p class="regular">
        As a Software Engineer Intern at <span class="work">Acumen Digital</span>, I had the opportunity
        to dive headfirst into the dynamic world of software development. Some
        key experiences and skills I gained include:
      </p>
    </div>
    <ul class="light-list">
      <li class="freight">
        <span class="work">Programming Expertise:</span> I honed my skills in various programming languages and frameworks like JavaScript Vue and Nuxt. This gave me a strong
        foundation for software development.
      </li>
      <li class="freight">
        <span class="work">Web Development:</span> I contributed to the creation of web applications,
        learning the ins and outs of front-end development,
        including HTML, CSS, and JavaScript.
      </li>
      <li class="freight">
        <span class="work">Agile Development:</span> I became proficient in agile methodologies, working
        closely with cross-functional teams and adapting to changing project
        requirements.
      </li>
      <li class="freight">
        <span class="work">Problem-Solving:</span> My time at Acumen Digital sharpened my problem-solving
        abilities, allowing me to develop efficient solutions to complex
        challenges.
      </li>
    </ul>
    </div>
</template>

<style scoped>
.light {
  height: auto;
  width: 60%;
  margin: 0 0 0 7px;
}

.light-header {
  height: 35%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: start;
  margin: 30px 0 0 0;
}

.span {
  color: rgb(195, 190, 190);
  font-size: 16px;
}

.break {
  color: rgb(148, 144, 144);
  margin: 0 0 0 0;
  font-family: "RobotoMono-VariableFont_wght";
  font-weight: 500;
  font-size: 16px;
  text-align: justify;
}

.light-list {
  color: #d8b5b5;
  list-style: none;
  margin: 0 0 0 0;
  padding: 0;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: start;
}

.wraith-point {
  margin: 0;
}

.wraith {
  color: #fff5ee;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 900;
  font-size: 20px;
  margin: 0;
}

.freight {
  color: #b79a9a;
  font-family: "Raleway-VariableFont_wght";
  font-size: 14px;
  text-align: justify;
  margin: 15px 0 0 0;
}

.regular {
  color: #d8b5b5;
  font-family: "Raleway-VariableFont_wght";
  font-size: 16px;
  text-align: justify;
  margin: 0 0 10px 0;
}

.work {
  color: #fff5ee;
}

@media (max-width: 450px) {
  .wraith{
    font-size: 18px;
  }

  .span{
    font-size: 14px;
  }

  .break{
    font-size: 14px;
  }

  .regular{
    font-size: 13px;
  }

  .freight{
    font-size: 11px;
  }

}
</style>