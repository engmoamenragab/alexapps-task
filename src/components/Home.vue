<template>
  <Header />
  <Table />
  <Footer />
  <Pagination />
</template>
<script>
import Header from "./Header.vue"
import Table from "./Table.vue"
import Footer from "./Footer.vue"
import Pagination from "./Pagination.vue"
export default {
  name: "Home",
  components: {
    Header,
    Table,
    Footer,
    Pagination
  }
}
</script>
<style scoped>

</style>
