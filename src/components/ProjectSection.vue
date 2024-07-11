<template>
  <section id="projects" class="projects bg-white rounded padding margin-bottom">
    <div class="container">
      <h2 class="text-bold margin-bottom">Projects</h2>
      <div class="project-list">
        <div class="project margin-bottom" v-for="project in projects" :key="project.id">
          <h3 class="text-bold">{{ project.name }}</h3>
          <p>{{ project.description }}</p>
          <a class="text-bold" :href="project.link" target="_blank">View Project</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          name: "LTeam Wine Map",
          description: "An interactive map application that helps users explore different wine regions and their unique characteristics. Built using Django and React.",
          link: "https://lteam-wine-map.fly.dev/"
        },
        {
          id: 2,
          name: "Equality Lesson",
          description: "A responsive landing page template created with HTML, CSS, and JavaScript. Showcases modern web design practices.",
          link: "https://equalitylesson.org/"
        },
        {
          id: 3,
          name: "CEDEM Quiz",
          description: "An interactive quiz platform developed using JavaScript and CSS. Provides a smooth user experience and proficiency in dynamic content handling.",
          link: "https://cedem.org.ua/tax-mechanism-online-test/"
        },
        {
          id: 4,
          name: "WeatherBot",
          description: "A chatbot application designed to provide real-time weather updates. Implemented using Node.js and Express.",
          link: "https://github.com/Nattalli/WeatherBot"
        }
      ]
    };
  }
};
</script>

<style scoped>
.projects {
  text-align: left;
}
.projects h2 {
  color: #252422;
}
.project-list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
.project {
  flex: 1 1 45%;
  padding: 20px;
  border: 1px solid #e0e0e0;
  border-radius: 10px;
  background-color: #ffffff;
  transition: box-shadow 0.3s;
}
.project h3 {
  margin-top: 0;
  color: #252422;
}
.project p {
  color: #403D39;
}
.project a {
  color: #EB5E28;
  text-decoration: none;
  transition: color 0.3s;
}
.project a:hover {
  color: #252422;
}
.project:hover {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
</style>
