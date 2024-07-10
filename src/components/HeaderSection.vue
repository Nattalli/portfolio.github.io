<template>
  <header className="header bg-white rounded padding box-shadow margin-bottom">
    <div className="container text-center">
      <h1>{{ name }}</h1>
      <h2>Fullstack developer (Python + JS)</h2>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      name: "Nataliia Zakharchuk"
    };
  }
};
</script>

<style scoped>
.header h1 {
  margin: 0;
  font-size: 2.5em;
  font-weight: bold;
}

.header h2 {
  margin: 0;
  font-size: 1.5em;
  color: #666666;
}
</style>
