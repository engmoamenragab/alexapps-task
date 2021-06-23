<template>
  <el-header class="header">
    <el-row :gutter="20">
      <el-col :span="16">
        <div class="grid-content bg-purple">
          <el-row :gutter="20">
            <el-col :span="8"
              ><div class="grid-content bg-purple">
                <Select text="إسم الفرع" /></div
            ></el-col>
            <el-col :span="8"
              ><div class="grid-content bg-purple">
                <Select text="المستوى" /></div
            ></el-col>
            <el-col :span="8"
              ><div class="grid-content bg-purple"><Date text="من تاريخ" /></div
            ></el-col>
          </el-row>
          <el-row :gutter="20">
            <el-col :span="8"
              ><div class="grid-content bg-purple">
                <Select text="مركز التكلفة" /></div
            ></el-col>
            <el-col :span="8"
              ><div class="grid-content bg-purple">
                <Date text="إلى تاريخ" /></div
            ></el-col>
          </el-row>
        </div>
      </el-col>
      <el-col class="header__left" :span="8">
        <div class="grid-content bg-purple">
          <el-row :gutter="20">
            <el-col :span="24">
              <div class="grid-content bg-purple">
                <el-button class="btn" type="danger">إظهار الحسابات التى رصيدها صفر</el-button>
              </div>
            </el-col>
          </el-row>
          <el-row :gutter="20">
            <el-col :span="12">
              <div class="grid-content bg-purple">
                <el-button class="btn" type="info">تضمين الأرصدة الإفتتاحية</el-button>
              </div>
            </el-col>
            <el-col :span="12">
              <div class="grid-content bg-purple">
                <el-button class="btn" type="info">تضمين قيمة المخزون</el-button>
              </div>
            </el-col>
          </el-row>
        </div>
      </el-col>
    </el-row>
  </el-header>
</template>
<script>
import Select from "./Select.vue";
import Date from "./Date.vue";
export default {
  name: "Header",
  components: {
    Select,
    Date,
  },
};
</script>
<style scoped>
.header {
  height: initial !important;
  margin-bottom: 20px;
}
.el-row {
  align-items: center;
}
.btn {
  margin: 10px 0;
  width: 100%;
  font-family: 'El Messiri', sans-serif;
}
</style>