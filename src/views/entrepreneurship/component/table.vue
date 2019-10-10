<template>
  <el-table
    :data="tableData"
    border
    style="width: 100%">
    <el-table-column
      fixed
      prop="date"
      label="姓名"
      width="150">
    </el-table-column>
    <el-table-column
      prop="name"
      label="所在机构"
      width="120">
    </el-table-column>
    <el-table-column
      prop="province"
      label="是否Alpha律所"
      width="120">
    </el-table-column>
    <el-table-column
      prop="city"
      label="职务"
      width="120">
    </el-table-column>
    <el-table-column
      prop="address"
      label="执业年限"
      width="300">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="手机号"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="最后更新时间"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="区域"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="邀请状态"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="邀请人"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="邀请记录"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="计划跟进日期"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="Alepha用户"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="Alepha用户最近登陆时间"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="近一个月使用次数"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="iCourt学员"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="参加课程次数"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="是否线上法学院"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="美国星学院"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="是否未来律所"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="标签"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="邀请级别"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="决策点"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="橙子手机"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="Alpha用户数"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="出生日期"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="最后联系时间"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="参加时间"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="参加人数"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="所在群"
      width="120">
    </el-table-column>
    <el-table-column
      prop="zip"
      label="备注"
      width="120">
    </el-table-column>
    <el-table-column
      fixed="right"
      label="操作"
      width="100">
      <template slot-scope="scope">
        <el-button @click="handleClick(scope.row)" type="text" size="small">查看</el-button>
        <el-button type="text" size="small">编辑</el-button>
      </template>
    </el-table-column>
  </el-table>
</template>
<script>
  export default {
      props:['tabdata'],
    methods: {
      handleClick(row) {
        console.log(row);
      }
    },

    data() {
      return {
        tableData: [{
          date: '2016-05-02',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1518 弄',
          zip: 200333
        }, {
          date: '2016-05-04',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1517 弄',
          zip: 200333
        }, {
          date: '2016-05-01',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1519 弄',
          zip: 200333
        }, {
          date: '2016-05-03',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1516 弄',
          zip: 200333
        }]
      }
    }
  }
</script>