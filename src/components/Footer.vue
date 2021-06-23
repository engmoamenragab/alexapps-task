<template>
  <el-row :gutter="10">
      <el-col :span="2">
        <div class="grid-content bg-purple">
          <el-button class="btn" type="primary">عرض</el-button>
        </div>
      </el-col>
      <el-col :span="2">
        <div class="grid-content bg-purple">
          <el-button class="btn" type="warning">طباعة PDF</el-button>
        </div>
      </el-col>
      <el-col :span="2">
        <div class="grid-content bg-purple">
          <el-button class="btn" type="warning">طباعة A4</el-button>
        </div>
      </el-col>
    </el-row>
</template>
<script>

export default {
  name: "Footer",
}
</script>
<style scoped>
.btn {
  width: 100%;
  font-family: 'El Messiri', sans-serif;
}
.el-row {
  padding: 30px 0;
  justify-content: flex-end;
}
</style>