<template>
  <div class="block">
    <el-pagination @size-change="handleSizeChange" @current-change="handleCurrentChange" v-model:currentPage="currentPage4"
      :page-sizes="[100, 200, 300, 400]" :page-size="100" layout="jumper, next, pager, prev, total, sizes" :total="400">
    </el-pagination>
  </div>
</template>
<script>

export default {
  name: "Pagination",
  methods: {
    handleSizeChange(val) {
      console.log(`${val} items per page`);
    },
    handleCurrentChange(val) {
      console.log(`current page: ${val}`);
    }
  },
  data() {
    return {
      currentPage1: 5,
      currentPage2: 5,
      currentPage3: 5,
      currentPage4: 4
    };
  }
  }
</script>