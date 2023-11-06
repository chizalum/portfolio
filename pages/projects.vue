<template>
  <div>
    <div class="last-layer">
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
  </div>
</template>

<script>
export default {
  name: "projects",
};
</script>

<style scoped>

.last-layer {
  display: flex;
  flex-direction: column;
  background: whitesmoke;
  height: auto;
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

@media (max-width: 450px) {
  .duties {
  width: 450px;
  height: 480px;
  background: url("~/assets/xyz.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 40px auto 0 auto;
}

  .duties1 {
  width: 450px;
  height: 480px;
  background: url("~/assets/robin-1.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 40px auto 0 auto;
}

.duties2 {
  width: 450px;
  height: 480px;
  background: url("~/assets/robin-2.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 40px auto 0 auto;
}

.duties3 {
  width: 450px;
  height: 480px;
  background: url("~/assets/robin-3.png") ;
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
  margin: 40px auto 0 auto;
}
}
</style>