<template>
  <el-table class="table" :data="tableData" :span-method="arraySpanMethod" stripe border style="width: 100%">
    <el-table-column prop="index" label="م" :min-width="10"></el-table-column>
    <el-table-column prop="date" label="إسم الحساب" :min-width="30"></el-table-column>
    <el-table-column prop="name" label="رصيد دائن" :min-width="30"></el-table-column>
    <el-table-column prop="address" label="رصيد مدين" :min-width="30"></el-table-column>
  </el-table>
</template>

<script>
export default {
  data() {
    return {
      tableData: [
        {
          index: "1",
          date: "إبراهيم السيد",
          name: "103276.86",
          address: "23649.13",
        },
        {
          index: "2",
          date: "إبراهيم السيد",
          name: "103276.86",
          address: "23649.13",
        },
        {
          index: "3",
          date: "إبراهيم السيد",
          name: "103276.86",
          address: "23649.13",
        },
        {
          index: "4",
          date: "إبراهيم السيد",
          name: "103276.86",
          address: "23649.13",
        },
        {
          index: "إجمالى ربح المتاجرة",
          date: "إبراهيم السيد",
          name: "103276.86",
          address: "23649.13",
        },
        {
          index: "الإجمالى",
          date: "إبراهيم السيد",
          name: "103276.86",
          address: "23649.13",
        },
      ],
    };
  },
  methods: {
    arraySpanMethod({ row, column, rowIndex, columnIndex }) {
        if (rowIndex == 4) {
          if (columnIndex === 0) {
            return [1, 2];
          } else if (columnIndex === 1) {
            return [0, 0];
          }
        }
        if (rowIndex == 5) {
          if (columnIndex === 0) {
            return [1, 2];
          } else if (columnIndex === 1) {
            return [0, 0];
          }
        }
      }
  }
};
</script>
<style>
.el-table td, .el-table th {
  text-align: center !important;
}
</style>