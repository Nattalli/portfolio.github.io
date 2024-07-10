<template>
  <section id="about" class="about bg-light rounded padding margin-bottom">
    <div class="container">
      <div class="about-content">
        <h2 class="text-bold margin-bottom">About Me</h2>
        <p>{{ aboutText }}</p>
        <ul>
          <li class="margin-bottom">📊 I love mathematics and study it in depth</li>
          <li class="margin-bottom">🔢 I’m also passionate about algorithms and continuously improve my skills in this area</li>
          <li class="margin-bottom">💬 My strengths include excellent soft skills and effective communication</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      aboutText: `I'm Nataliia Zakharchuk, a Python developer with almost 3 years of experience. I started my career as a backend developer and have evolved into a full-stack developer. My skill set includes:
      - Backend: Django, Django REST Framework
      - Frontend: React, basic Vue.js, JavaScript, CSS, HTML
      - Server-side: Express, Node.js`
    };
  }
};
</script>

<style scoped>
.about {
  text-align: left;
}
.about .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
}
.about-content {
  flex: 1;
  text-align: left;
  padding-right: 20px;
}
.about-content h2 {
  color: #333333;
}
.about-content p {
  font-size: 18px;
  color: #666666;
}
.about-content ul {
  list-style: none;
  padding: 0;
}
.about-content ul li {
  font-size: 16px;
  color: #333333;
}
.about-photo img {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
}
</style>
