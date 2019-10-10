<template>
  <div>
    <div class="selectbox" :content="content">
      <ul v-for="slide in content" :key="slide.id">
        <li v-text="slide.title"></li>
        <li v-if="slide.ipt">
          <el-input :placeholder="slide.name"></el-input>
        </li>
        <li v-else-if="slide.num">
          <vselect :vname="slide.name"/>
        </li>
        <li v-else-if="slide.type">
          <el-select :placeholder="slide.name">
            <el-option></el-option>
          </el-select>
        </li>
        <li v-else-if="slide.timer">
          <el-date-picker v-model="value1" type="date" :placeholder="slide.name"></el-date-picker>
        </li>
      </ul>
    </div>
    <!-- <div class="btnbox">
      <div class="leftbtn">
        <button>+新增用户</button>
        <button>今日跟进</button>
      </div>
      <div class="rightbtn">
        <button>搜索</button>
        <button>重置</button>
      </div>
    </div> -->
    <vbtn/>
    <div class="tablebox">
        <vtable :tabdata="content"/>
    </div>
  </div>
</template>
<script>
import list from "../../../mock/entrepreneur.json";
import vselect from "./component/select";
import vbtn from './component/bottom'
import vtable from './component/table'
export default {
  components: {
    vselect,
    vbtn,
    vtable
  },
  data() {
    return {
      content: []
    };
  },
  created() {
    this.content = list;
  }
};
</script>
<style lang="scss" scoped>
* {
  list-style: none;
  font-size: 12px;
}
.selectbox {
  width: 100%;
  height: auto;
  ul {
    height: 50px;
    width: 25%;
    float: left;
    li {
      margin: 5px 0;
    }
  }
}
.tablebox {
  height: auto;
  clear: both;
}
</style>
