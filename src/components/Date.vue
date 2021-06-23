<template>
  <div>{{ text }}</div>
  <div class="block">
    <el-date-picker
      v-model="value2"
      type="date"
      placeholder="Pick a day"
      :disabled-date="disabledDate"
      :shortcuts="shortcuts"
    >
    </el-date-picker>
  </div>
</template>

<script>
export default {
  name: "Date",
  props: ["text"],
  data() {
    return {
      disabledDate(time) {
        return time.getTime() > Date.now();
      },
      shortcuts: [
        {
          text: "Today",
          value: new Date(),
        },
        {
          text: "Yesterday",
          value: (() => {
            const date = new Date();
            date.setTime(date.getTime() - 3600 * 1000 * 24);
            return date;
          })(),
        },
        {
          text: "A week ago",
          value: (() => {
            const date = new Date();
            date.setTime(date.getTime() - 3600 * 1000 * 24 * 7);
            return date;
          })(),
        },
      ],
      value1: "",
      value2: "",
    };
  },
};
</script>