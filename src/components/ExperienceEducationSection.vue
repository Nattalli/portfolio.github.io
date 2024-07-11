<template>
  <section id="experience-education" class="experience-education bg-white rounded padding margin-bottom">
    <div class="container">
      <div class="experience">
        <h2 class="text-bold margin-bottom">Work Experience</h2>
        <div class="experience-item margin-bottom" v-for="job in jobs" :key="job.id">
          <h3>{{ job.period }}</h3>
          <h4 class="text-bold">{{ job.title }}</h4>
          <p>{{ job.description }}</p>
          <p><strong>Tech stack:</strong> {{ job.techStack }}</p>
        </div>
      </div>
      <div class="education">
        <h2 class="text-bold margin-bottom">Education</h2>
        <div class="education-item margin-bottom" v-for="education in educations" :key="education.id">
          <h3>{{ education.period }}</h3>
          <h4 class="text-bold">{{ education.degree }}</h4>
          <p>{{ education.institution }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      jobs: [
        {
          id: 1,
          period: "07/2023 - till now",
          title: "Fullstack developer at INFOTECH",
          description: "Development and maintenance of the existing healthcare system: modifying page styles to align with the new design, creating new pages, and enhancing the functionality of existing features.",
          techStack: "Python, Django, jQuery, JS, React, Docker, jasper"
        },
        {
          id: 2,
          period: "08/2022 - 07/2023",
          title: "Fullstack developer and Python mentor at Mate academy",
          description: "Created webhook system with usage of AWS SQS, DRF, and Next.js; Python course improvement with theory coverage, mentorship of Python students.",
          techStack: "Python, Django, DRF, AWS, Next.js, Docker"
        },
        {
          id: 3,
          period: "11/2021 - 06/2022",
          title: "Python backend developer at PM Digital Transformation",
          description: "CRM-systems creating; online-shop, blog, and charity project backend part, admin panel customizing.",
          techStack: "Python, Django, DRF"
        }
      ],
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
.experience-education {
  text-align: left;
}
.container {
  display: flex;
  justify-content: space-between;
}
.experience, .education {
  flex: 1;
  margin-right: 20px;
}
.experience h2, .education h2 {
  color: #252422;
}
.experience-item h3, .education-item h3 {
  margin-bottom: 5px;
  color: #403D39;
}
.experience-item h4, .education-item h4 {
  margin: 0;
  font-size: 1.2em;
  color: #EB5E28;
}
.experience-item p, .education-item p {
  margin: 5px 0;
  color: #403D39;
}
</style>
