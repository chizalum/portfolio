<template>
  <div class="light">
    <div class="light-header">
      <div class="wraith-point">
        <P class="wraith"
          >Nasco Household products<span class="span"
            ><br>Quality assurance personnel</span
          ></P
        >
        <p class="break">2019</p>
      </div>
      <p class="regular">
        My time at, <span class="work">Nasco</span> a household goods
        manufacturing company, gave me valuable insights into the manufacturing
        sector and allowed me to apply my technology skills in a different
        context:
      </p>
    </div>
    <ul class="light-list">
      <li class="freight">
        <span class="work">Process Optimization:</span> I leveraged my technical skills to optimize
        manufacturing processes, reducing waste and increasing efficiency.
      </li>
      <li class="freight">
        <span class="work">Data Analysis:</span> I collected and analyzed data to improve product quality
        and production timelines, showcasing my ability to use technology for
        data-driven decision-making.
      </li>
      <li class="freight">
        <span class="work">Supply Chain Management:</span> I gained knowledge of supply chain operations and used software solutions to enhance inventory management.
      </li>
    </ul>
  </div>
</template>

<style scoped>
.light {
  height: 480px;
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
  margin: 0 0 0 0;
  font-size: 16px;
  color: rgb(195, 190, 190);
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
</style>