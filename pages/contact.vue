<template>
  <div class="first-div">
    <div class="grid-container">
      <div
        class="second-div"
        v-for="(details, index) in contact"
        :key="index"
        @mouseover="startHover(index)"
        @mouseleave="stopHover(index)"
      >
        <a :href="details.link" target="blank">
          <img class="symbols" :src="details.heart" />
        </a>
        <a class="boxx" :href="details.link" target="blank">
          <button class="text" :class="{ highlight: details.textbox }">{{ details.name }}</button>
        </a>
        <p class="info" v-if="details.textbox">{{ details.info }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      texting: false,
      contact: [
        {
          index: 1,
          name: "Call Me",
          heart: "phone-504.svg",
          link: "tel:+2348126337630",
          isActiveMobile: false,
          info: "CALL",
          textbox: false,
        },
        {
          index: 2,
          name: "Email Me",
          heart: "email.svg",
          link: "mailto:joshuaegbuonu@gmail.com",
          isActiveMobile: false,
          info: "joshuaegbuonu@gmail.com",
          textbox: false,
        },
        {
          index: 3,
          name: "linkedin",
          heart: "linkdin.svg",
          link: "https://www.linkedin.com/in/joshua-egbuonu-8b1479228",
          isActiveMobile: false,
          info: "https://www.linkedin.com/in/joshua-egbuonu-8b1479228",
          textbox: false,
        },
        {
          index: 4,
          name: "Github",
          heart: "github.svg",
          link: "https://github.com/chizalum",
          isActiveMobile: false,
          info: "https://github.com/chizalum",
          textbox: false,
        },
        {
          index: 5,
          name: "Send a text",
          heart: "text.svg",
          link: "sms:08126337630?body= I'll like to make an enquiry about your services",
          isActiveMobile: false,
          info: "TEXT",
          textbox: false,
        },
      ],
    };
  },

  methods: {
    startHover(index) {
      this.contact[index].textbox = true;
    },
    stopHover(index) {
      this.contact[index].textbox = false;
    },
  },
};
</script>

<style scoped>
.first-div {
  display: flex;
  flex-direction: row;
  margin: 0 0 0 0;
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
  background: linear-gradient(180deg, #f5f5f5, #e9ddd4);
  align-items: center;
  justify-content: center;
  text-align: center;
}

.second-div {
  display: flex;
  flex-direction: column;
  margin: 70px 0 0 0;
  width: 300px;
  height: 30vh;
  background: linear-gradient(180deg, #f5f5f5, #c2c2c2);
  align-items: center;
  justify-content: center;
  text-align: center;
  backdrop-filter: saturate(180%) blur(10px);
}

.boxx {
  margin: 25px 0 0 0;
  word-wrap: break-word;
  cursor: pointer;
}

.text {
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 18px;
  margin: 25px 0 0 0;
  text-decoration: none;
  color: black;
  word-wrap: break-word;
  background: rgb(147, 155, 146);
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.highlight{
  font-family: "RobotoMono-VariableFont_wght";
  font-size: 18px;
  text-decoration: none;
  color: black;
  word-wrap: break-word;
  background: rgb(159, 206, 142);
  border: none;
  width: 100%;
  height: 30px;
  border-radius: 4px;
  cursor: pointer;
}

.info {
  word-wrap: break-word;
  font-family: "Raleway-VariableFont_wght";
  font-weight: 400;
  font-size: 12px;
  margin: 30px auto 0 auto;
  padding: 0 auto 0 auto;
}

@media (max-width: 950px) {
  .grid-container {
  display: grid;
  grid-template-columns: 300px 300px;
  width: 92%;
  justify-content: center;
  row-gap: 70px;
  column-gap: 12%;
  margin: auto auto auto auto;
}
}


@media (max-width: 650px) {

  .grid-container {
  display: grid;
  grid-template-columns: 300px;
  width: 92%;
  justify-content: center;
  row-gap: 70px;
  column-gap: 12%;
  margin: auto auto auto auto;
}
}
</style>