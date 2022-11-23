<template>
  <div class="first-div">
    <div class="grid-container">
      <div class="second-div" v-for="(details, index) in contact" :key="index" >
        <a :href="details.link" target="blank">
          <img class="symbols" :src="details.heart" />
        </a>
        <a class="text" :href="details.link" target="blank">
          <p class="name">{{ details.name }}</p>
        </a>
        <p class="info">{{details.info}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      contact: [
        {
          index: 1,
          name: "Call Me",
          heart: "phone-504.svg",
          link: "tel:+2348126337630",
          isActiveMobile: false,
          info: "CALL",
        },
        {
          index: 2,
          name: "Email Me",
          heart: "email.svg",
          link: "mailto:joshuaegbuonu@gmail.com",
          isActiveMobile: false,
          info: "joshuaegbuonu@gmail.com",
        },
        {
          index: 3,
          name: "linkedin",
          heart: "linkdin.svg",
          link: "https://www.linkedin.com/in/joshua-egbuonu-8b1479228",
          isActiveMobile: false,
          info: "https://www.linkedin.com/in/joshua-egbuonu-8b1479228",
        },
        {
          index: 4,
          name: "Github",
          heart: "github.svg",
          link: "https://github.com/chizalum",
          isActiveMobile: false,
          info: "https://github.com/chizalum"
        },
        {
          index: 4,
          name: "Send a text",
          heart: "text.svg",
          link: "sms:08126337630?body= I'll like to make an enquiry about your services",
          isActiveMobile: false,
          info: "TEXT",
        },
      ],
    };
  },
};
</script>

<style scoped>
.first-div {
  display: flex;
  flex-direction: row;
  margin: 0 0 0 0;
  background: whitesmoke;
  width: 100vw;
  height: 100vh;
  justify-content: center;
  align-items: center;
}

.grid-container {
  display: grid;
  grid-template-columns: 300px 300px 300px;
  width: 92%;
  justify-content: center;
  row-gap: 70px;
  column-gap: 12%;
  margin: auto auto auto auto;
}
.symbols {
  margin: 0 0 0 0;
  width: 34px;
  height: 34px;
}

.second-div:hover {
  display: flex;
  flex-direction: column;
  margin: 70px 0 0 0;
  width: 300px;
  height: 30vh;
  background: linear-gradient(180deg,#F5F5F5, #E9DDD4);
  align-items: center;
  justify-content: center;
}

.second-div{
  display: flex;
  flex-direction: column;
  margin: 70px 0 0 0;
  width: 300px;
  height: 30vh;
  background: linear-gradient(180deg,#F5F5F5, #C2C2C2);
  align-items: center;
  justify-content: center;
}

.text {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 18px;
  margin: 25px 0 0 0;
  text-decoration: none;
  color: black;
  word-wrap: break-word;
}

.name{

}

.info{
  word-wrap: break-word;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 13px;
  margin: 0 0 0 0;
}
</style>