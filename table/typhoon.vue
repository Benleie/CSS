<template>
  <div class='table-wrapper'>
     <el-table
      :data="tableData"
      stripe
      border
      :header-cell-style="headerStyle"
      class="typhoon-table">
      <el-table-column
        prop="year"
        label="年份"
        align="center"
        width="150">
      </el-table-column>
      <el-table-column
        prop="id"
        label="台风编号"
        align="center"
        width="150">
      </el-table-column>
      <el-table-column
        prop="name"
        label="台风名"
        align="center">
      </el-table-column>
    </el-table>
   
  </div>
</template>

<script>
  export default {
    components: {},
    data() {
      return {
        tableData: [
          { year: "2020", id: "2019", name: "鹦鹉" },
          { year: "2020", id: "2019", name: "鹦鹉" },
          { year: "2020", id: "2019", name: "鹦鹉" },
          { year: "2020", id: "2019", name: "鹦鹉" },
          { year: "2020", id: "2019", name: "鹦鹉" },
          { year: "2020", id: "2019", name: "鹦鹉" },
          { year: "2020", id: "2019", name: "鹦鹉" }
        ],
        headerStyle: {
          backgroundColor: '#0f345C',
          color: '#ffffff',
          fontWeight: 600
        },
      };
    },
    methods: {},
  }
</script>

<style scoped>

.typhoon-table {
  margin: 50px 0 0 100px;
  width: 460px;
  /* border: 3px solid salmon; */
}
</style>
<style>
/* 表头错位 */
.typhoon-table th.gutter {
  display: table-cell !important;
}

.typhoon-table tr {
  background-color: #062545;
  color: #ffffff;
}
/* 修改striped行颜色 */
.typhoon-table .el-table__body tr.el-table__row--striped td{
  background-color: #06284C;
  color: #ffffff;
}
/* hover */
.el-table--enable-row-hover .el-table__body tr:hover td{
  background-color: darkgrey;
}

.typhoon-table td, .typhoon-table th.is-leaf {
  border-bottom: none;
}


/* .typhoon-table td, .typhoon-table th{
  border-right: 1px solid lightcyan;
} */
</style>