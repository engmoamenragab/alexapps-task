<template>
  <Header />
  <Table />
  <Footer />
  <Pagination />
</template>

<script>
import Header from "./components/Header.vue";
import Table from "./components/Table.vue";
import Footer from "./components/Footer.vue";
import Pagination from "./components/Pagination.vue";
export default {
  name: "App",
  components: {
    Header,
    Table,
    Footer,
    Pagination,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=El+Messiri:wght@400;500;600;700&display=swap');
#app {
  font-family: 'El Messiri', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
