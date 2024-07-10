<template>
  <section id="education" class="education bg-light rounded padding margin-bottom">
    <div class="container">
      <h2 class="text-bold margin-bottom">Education</h2>
      <div class="education-item margin-bottom" v-for="education in educations" :key="education.id">
        <h3 class="text-italic">{{ education.period }}</h3>
        <h4 class="text-bold">{{ education.degree }}</h4>
        <p>{{ education.institution }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      educations: [
        {
          id: 1,
          period: "10/2023 - 05/2025",
          degree: "Master’s degree at Faculty of Computer Science and Cybernetics",
          institution: "Taras Shevchenko National University of Kyiv"
        },
        {
          id: 2,
          period: "09/2019 - 06/2023",
          degree: "Bachelor degree at Faculty of Computer Science and Cybernetics",
          institution: "Taras Shevchenko National University of Kyiv"
        }
      ]
    };
  }
};
</script>

<style scoped>
.education {
  text-align: left;
}
.education h2 {
  color: #333333;
}
.education-item h3 {
  margin-bottom: 5px;
  color: #e63946;
}
.education-item h4 {
  margin: 0;
  font-size: 1.2em;
  color: #333333;
}
.education-item p {
  margin: 5px 0;
  color: #666666;
}
</style>
