<template>
  <div>
    <v-app-bar>
      <v-toolbar-title>
        <v-btn class="v-btn-title" href="/">REENPRESENTS</v-btn>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <ul>
        <a href="/about">About</a>
        <a href="/recomendation">Recomendation</a>
        <a href="/place">Place Addres</a>
      </ul>
    </v-app-bar>
  </div>
</template>
<script>
export default {
  name: "App",
  data: () => {
    return {};
  },
  beforeCreated() {
    alert("hallo");
  }
};
</script>
<style scoped>
.v-btn-title {
  font-display: Krona One;
  font-size: 24px;
  color: aliceblue;
  background-color: #97e4e0 !important;
}
ul {
  margin-right: 30px;
}
a {
  font-family: Poppins;
  font-size: 20px;
  margin: 0 10px 0 10px;
  text-decoration: none;
}
.v-btn-title {
  margin-left: 40px !important;
}
</style>