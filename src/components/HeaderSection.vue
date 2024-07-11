<template>
  <header class="header bg-white rounded padding box-shadow margin-bottom">
    <div class="container text-center">
      <div class="header-content">
        <div>
          <h1>{{ name }}</h1>
          <h2>Fullstack developer (Python + JS)</h2>
        </div>
        <div class="contact">
          <ul>
            <li>Email: <a :href="'mailto:' + email">{{ email }}</a></li>
            <li>GitHub: <a :href="github" target="_blank">{{ github }}</a></li>
            <li>Telegram: <a :href="telegram" target="_blank">{{ telegram }}</a></li>
            <li>Phone: {{ phone }}</li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      name: "Nataliia Zakharchuk",
      email: "zakharchuk.nataliiaa@gmail.com",
      github: "https://github.com/Nattalli",
      telegram: "https://t.me/natalllii",
      phone: "+380666874067"
    };
  }
};
</script>

<style scoped>
.header {
  padding: 20px 0;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header h1 {
  margin: 0;
  font-size: 2.5em;
  font-weight: bold;
}
.header h2 {
  margin: 0;
  font-size: 1.5em;
  color: #403D39;
}
.contact ul {
  text-align: left;
  list-style: none;
  padding: 0;
  margin: 0;
  font-size: 1em;
  color: #333333;
}
.contact ul li {
  margin-bottom: 5px;
}
.contact ul li a {
  color: #EB5E28;
  text-decoration: none;
  transition: color 0.3s;
}
.contact ul li a:hover {
  color: #252422;
}
</style>
