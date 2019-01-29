<template>
  <div class="table">
    <el-form>
      <el-form-item >
        <el-button size="small" @click="getDataList()" class="btn-right">查询全部</el-button>
        <el-button size="small" type="primary" @click="addRow()" class="btn-right">新增</el-button>
      </el-form-item>
    </el-form>
    <el-table
      :data="tableData"
      ref="table"
      style="width: 100%">
      <el-table-column label="名称">
        <template slot-scope="scope">
          <el-input v-model="scope.row.address"></el-input>
        </template>
      </el-table-column>
      <el-table-column width="240" label="日期" >
        <template slot-scope="scope">
          <el-input v-model="scope.row.name"></el-input>
        </template>
      </el-table-column>
      <el-table-column width="240" label="投资额（万元）" >
        <template slot-scope="scope">
          <el-input v-model="scope.row.loveer"></el-input>
        </template>
      </el-table-column>
      <el-table-column width="240" prop="name" label="开发人" >
        <template slot-scope="scope">
          <el-input v-model="scope.row.weather"></el-input>
        </template>
      </el-table-column>
      <el-table-column width="240" label="备注" >
        <template slot-scope="scope">
          <el-input v-model="scope.row.phone" ></el-input>
        </template>
      </el-table-column>
      <el-table-column label="操作">
        <template slot-scope="scope">
          <el-button size="mini" @click="addOrUpdateHandle(scope.row.custId)">修改</el-button>
          <el-button size="mini" type="danger" @click="deleteHandle(scope.row.custId)">删除</el-button>
          <el-button size="mini" type="danger" @click="deleteHandle(scope.row.custId)">移除</el-button>
          <el-button size="mini" type="danger" @click="deleteHandle(scope.row.custId)">变更记录</el-button>
        </template>
      </el-table-column>
    </el-table>
  </div>
</template>

<script>
  export default {
    name: 'investor-info',
    data () {
      return {
        tableData: [{
          rowNum: 1,
          address: '西安城墙',
          name: '小哥',
          weather: '下雪',
          phone: '0771-5201314',
          date: '2016-11-22',
          mdate: '2018-04-10',
          loveer: '甜甜圈'
        }, {
          rowNum: 2,
          address: '西安城墙',
          name: '小哥',
          weather: '下雪',
          phone: '0771-5201314',
          date: '2016-11-22',
          mdate: '2018-04-10',
          loveer: '甜甜圈'
        }, {
          rowNum: 3,
          address: '西安城墙',
          name: '小哥',
          weather: '下雪',
          phone: '0771-5201314',
          date: '2016-11-22',
          mdate: '2018-04-10',
          loveer: '甜甜圈'
        }, {
          rowNum: 4,
          address: '西安城墙',
          name: '小哥',
          weather: '下雪',
          phone: '0771-5201314',
          date: '2016-11-22',
          mdate: '2018-04-10',
          loveer: '甜甜圈'
        }, {
          rowNum: 5,
          address: '西安城墙',
          name: '小哥',
          weather: '下雪',
          phone: '0771-5201314',
          date: '2016-11-22',
          mdate: '2018-04-10',
          loveer: '甜甜圈'
        }],
        selectlistRow: []
      }
    },
    methods: {
      addRow () {
        var list = {
          rowNum: '',
          address: this.address,
          name: this.name,
          weather: this.weather,
          phone: this.phone,
          date: this.date,
          mdate: this.mdate,
          loveer: this.loveer}
        this.tableData.unshift(list)
      }
    }
  }
</script>

<style>
  .btn-right{
    float: right;margin: 0 10px 0 10px;
  }
  .table-column{
    width: 50px;
  }
</style>
