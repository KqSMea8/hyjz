<template>
  <el-form :inline="true" :model="baseInfo" label-width="120px" style="width: 1450px">
    <el-form-item label="名称">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="手机">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="地区">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="开始日期">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="结束日期">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="开发人">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="负责人">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="交易员">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="初始市值">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="本金">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item label="备注">
      <el-input v-model="baseInfo.user" class="detail-input"></el-input>
    </el-form-item>
    <el-form-item>
      <el-button type="primary" >查询</el-button>
    </el-form-item>
  </el-form>
</template>


<script>
  export default {
    name: 'base-info',
    data () {
      return {
        baseInfo: {}
      }
    },
    method: function () {
    }
  }
</script>


<style>
  .detail-input{
    width: 300px;
  }
</style>
