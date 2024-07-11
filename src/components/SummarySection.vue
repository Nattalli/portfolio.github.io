<template>
  <section id="summary-about" class="summary-about bg-white rounded padding margin-bottom">
    <div class="container">
      <div class="summary">
        <h2 class="text-bold margin-bottom">Summary</h2>
        <p>
          I am a highly-motivated Software Developer with almost 3 year of commercial experience in Python back-end developing and 2 year in frontend development with JS, React, jQuery and Next.js. I’m a quick learner, therefore I'm looking for new opportunities in a company where I will fulfill my true potential as a fullstack developer.
        </p>
      </div>
      <div class="about">
        <h2 class="text-bold margin-bottom">About Me</h2>
        <p>
          📊 I love mathematics and study it in depth<br>
          🔢 I’m also passionate about algorithms and continuously improve my skills in this area<br>
          💬 My strengths include excellent soft skills and effective communication
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
};
</script>

<style scoped>
.summary-about {
  text-align: left;
}
.container {
  display: flex;
  justify-content: space-between;
}
.summary, .about {
  flex: 1;
  margin-right: 20px;
}
.summary h2, .about h2 {
  color: #403D39;
}
.summary p, .about p {
  font-size: 1.1em;
  color: #403D39;
}
.about p {
  margin-top: 0;
}
</style>
