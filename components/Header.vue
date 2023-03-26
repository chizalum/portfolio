<template>
  <div>
    <div class="navigation">
      <nuxt-link to="/" class="nav-link">Home</nuxt-link>
      <nuxt-link to="/about" class="nav-link">About</nuxt-link>
      <nuxt-link to="/projects" class="nav-link">Projects</nuxt-link>
      <nuxt-link to="/contact" class="nav-link">Contact</nuxt-link>
    </div>
     <div class="footer">
      <div class="sub-foot">
      <img class="symbols3" src="plant.svg">
      </div>
      <div class="sub-foot1">
         <a
          href="https://github.com/chizalum"
          download
          target="blank"
        >
          <img class="symbols" src="github.svg">
        </a>
         <a
          href="https://www.linkedin.com/in/joshua-egbuonu-8b1479228"
          download
          target="blank"
        >
          <img class="symbols3" src="linkdin.svg">
        </a>
      </div>
      </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};


</script>

<style scoped>
.navigation {
  display: flex;
  flex-direction: row;
  margin: 0 0 0 0;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 65px;
  align-items: center;
  justify-content: flex-end;
  z-index: 10000;
}


.nav-link {
  color: rgb(119, 107, 92);
  margin: auto 50px auto 0;
  text-decoration: none;
  font-family: "RubikMaze";
  font-size: 18px;
}

a.nuxt-link-exact-active {
  color: rgb(68, 149, 68);
  font-weight: 700;
  font-size: 22px;
}

.footer{
  display: flex;
  flex-direction: row;
  height: 35px;
  width: 100vw;
  position: fixed;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: space-between;
  white-space: nowrap;
  z-index: 10000;
}

.symbols{
  height: 20px;
  width: 20px;
  margin: auto 0 auto 0;
}

.symbols3{
  height: 30px;
  width: 30px;
  margin: auto 0 auto 18px;
}

.sub-foot{
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
}

.sub-foot1{
  display: flex;
  flex-direction: row;
  width: 150px;
  justify-content: space-evenly;
  align-items: center;
}

@media (max-width: 600px){
  .navigation {
  display: flex;
  flex-direction: row;
  margin: 0 0 0 0;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 65px;
  background: rgb(208, 225, 201);
  align-items: center;
  justify-content: center;
  z-index: 10000;
}

.nav-link {
  color: rgb(119, 107, 92);
  margin: auto auto auto auto;
  text-decoration: none;
  font-family: "RubikMaze";
  font-size: 14px;
}

a.nuxt-link-exact-active {
  color: #c69f73;
  font-weight: 700;
  font-size: 18px;
}
}
</style>