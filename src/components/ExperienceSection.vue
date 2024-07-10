<template>
  <section id="experience" class="experience bg-white rounded padding margin-bottom">
    <div class="container">
      <h2 class="text-bold margin-bottom">Work Experience</h2>
      <div class="experience-item margin-bottom" v-for="job in jobs" :key="job.id">
        <h3 class="text-italic">{{ job.period }}</h3>
        <h4 class="text-bold">{{ job.title }}</h4>
        <p>{{ job.description }}</p>
        <p><strong>Tech stack:</strong> {{ job.techStack }}</p>
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
      ]
    };
  }
};
</script>

<style scoped>
.experience {
  text-align: left;
}
.experience h2 {
  color: #333333;
}
.experience-item h3 {
  margin-bottom: 5px;
  color: #e63946;
}
.experience-item h4 {
  margin: 0;
  font-size: 1.2em;
  color: #333333;
}
.experience-item p {
  margin: 5px 0;
  color: #666666;
}
</style>
