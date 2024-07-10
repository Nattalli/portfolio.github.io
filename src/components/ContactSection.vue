<template>
  <section id="contact" class="contact bg-white rounded padding margin-bottom">
    <div class="container">
      <h2 class="text-bold margin-bottom">Contact</h2>
      <ul>
        <li class="margin-bottom">Email: <a :href="'mailto:' + email">{{ email }}</a></li>
        <li class="margin-bottom">GitHub: <a :href="github" target="_blank">{{ github }}</a></li>
        <li class="margin-bottom">Telegram: <a :href="telegram" target="_blank">{{ telegram }}</a></li>
        <li class="margin-bottom">Phone: {{ phone }}</li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      email: "zakharchuk.nataliiaa@gmail.com",
      github: "https://github.com/Nattalli",
      telegram: "https://t.me/natalllii",
      phone: "+380666874067"
    };
  }
};
</script>

<style scoped>
.contact {
  text-align: left;
}
.contact h2 {
  color: #333333;
}
.contact ul {
  list-style: none;
  padding: 0;
  font-size: 1.1em;
  color: #666666;
}
.contact ul li {
  margin-bottom: 10px;
}
.contact ul li a {
  color: #e63946; /* Червоний колір */
  text-decoration: none;
  transition: color 0.3s;
}
.contact ul li a:hover {
  color: #d62828; /* Темно-червоний колір при наведенні */
}
</style>
