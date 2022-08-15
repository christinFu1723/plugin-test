<template>
  <div>
    <div class="hello">文立测试包</div>
    <el-input v-model="input" placeholder="请输入内容"></el-input>
    <el-date-picker v-model="value1" type="date" placeholder="选择日期">
    </el-date-picker>
  </div>
</template>

<script>
import { Input, DatePicker } from "element-ui";
import "element-ui/lib/theme-chalk/index.css";

export default {
  name: "HelloWorld",
  components: {
    "el-input": Input,
    "el-date-picker": DatePicker,
  },
  props: {
    msg: String,
  },
  data() {
    return {
      input: "",
      value1: "",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
