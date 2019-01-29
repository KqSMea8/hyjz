<template>
  <div>
    <div>
      <h3>基本信息</h3>
      <base-info></base-info>
    </div>
    <div>
      <h3>投资者信息</h3>
      <investor-info></investor-info>
    </div>
  </div>


</template>

<script>
  import BaseInfo from './component/base-info'
  import InvestorInfo from './component/investor-info'
  export default {
    data () {
      return {
      }
    },
    components: {
      BaseInfo,
      InvestorInfo
    }
  }
</script>

<style>

</style>
