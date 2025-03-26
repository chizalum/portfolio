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
