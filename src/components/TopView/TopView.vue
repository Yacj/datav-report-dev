<template>
  <div id="TopView">
    <el-row :gutter="20">
      <el-col :span="6">
        <el-card shadow="hover">
          <total-sales/>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <total-orders/>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
         <today-user/>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <total-users/>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import TotalSales from "@/components/TotalSales/TotalSales";
import TotalOrders from "@/components/TotalOrders/TotalOrders";
import TotalUsers from "@/components/TotalUsers/TotalUsers";
import TodayUser from "@/components/TodayUser/TodayUser";
export default {
  name: "TopView",
  components: {TodayUser, TotalUsers, TotalOrders, TotalSales}
}
</script>

<style scoped lang="scss">

</style>