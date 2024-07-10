<template>
  <div id="app">
    <HeaderSection/>
    <div className="main-content">
      <TechnologiesSection/>
      <SummarySection/>
      <AboutSection/>
      <ExperienceSection/>
      <EducationSection/>
      <ProjectSection/>
      <ContactSection/>
    </div>
  </div>
</template>

<script>
import HeaderSection from './components/HeaderSection.vue';
import TechnologiesSection from './components/TechnologiesSection.vue';
import SummarySection from './components/SummarySection.vue';
import AboutSection from './components/AboutSection.vue';
import ExperienceSection from './components/ExperienceSection.vue';
import EducationSection from './components/EducationSection.vue';
import ContactSection from './components/ContactSection.vue';
import ProjectSection from './components/ProjectSection.vue';

export default {
  components: {
    HeaderSection,
    TechnologiesSection,
    SummarySection,
    AboutSection,
    ExperienceSection,
    EducationSection,
    ContactSection,
    ProjectSection
  }
};
</script>

<style>
body {
  font-family: 'Helvetica Neue', Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: #f7f7f7;
  color: #333333;
}

.main-content {
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: 20px;
}

.bg-white {
  background-color: #ffffff;
}

.bg-light {
  background-color: #f7f7f7;
}

.padding {
  padding: 20px;
}

.margin-bottom {
  margin-bottom: 20px;
}

.text-left {
  text-align: left;
}

.text-center {
  text-align: center;
}

.text-bold {
  font-weight: bold;
}

.text-italic {
  font-style: italic;
}

.rounded {
  border-radius: 10px;
}

.box-shadow {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

ul {
  list-style: none;
  padding: 0;
}

a {
  color: #e63946;
  text-decoration: none;
  transition: color 0.3s;
}

a:hover {
  color: #d62828;
}
</style>
