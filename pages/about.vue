<template>
    <div>
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
            <button class="experience1" :class="{ rotate: showDetails, highlight: highDetails }" @click="writeDetails"
              @mouseover="startHover()" @mouseleave="stopHover()">
              <p class="org" :class="{ bold: showDetails }">Acumen Digital</p>
            </button>

            <button class="experience" :class="{ rotate: showDetails1, highlight: highDetails1 }" @click="writeDetails1"
              @mouseover="startHover1()" @mouseleave="stopHover1()">
              <p class="org" :class="{ bold: showDetails1 }">
                Nigeria Security Printing and Minting
              </p>
            </button>
            <button class="experience" :class="{ rotate: showDetails2, highlight: highDetails2 }" @click="writeDetails2"
              @mouseover="startHover2()" @mouseleave="stopHover2()">
              <p class="org" :class="{ bold: showDetails2 }">Nasco</p>
            </button>
          </div>
          <hr class="ruling" />
          <Acumen v-if="showAcumen" class="insert" :class="{ bring: showAcumen }"></Acumen>
          <Nasco v-if="showNasco" class="insert" :class="{ bring: showNasco }"></Nasco>
          <Nspm v-if="showNspm" class="insert" :class="{ bring: showNspm }"></Nspm>
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