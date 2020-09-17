<template>
  <common-card
      title="累计销售额"
      value="￥32">
    <template>
      <div class="compare-wrapper">
        <div class="compare">
          <span>日同比</span>
          <span class="emphasis">7.33%</span>
          <div class="increase"></div>
        </div>
        <div class="compare">
          <span>月同比</span>
          <span class="emphasis">7.33%</span>
          <div class="decrease"></div>
        </div>
      </div>
    </template>
    <template slot="footer">
      <span>昨日销售额</span>
      <span class="emphasis">￥ 30,000,000</span>
    </template>
  </common-card>
</template>

<script>
import commonCard from "@/mixins/commonCard";

export default {
  name: "TotalSales",
  mixins: [commonCard]
}
</script>

<style scoped lang="scss">
.compare-wrapper{
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  .compare{
    display: flex;
    align-items: center;
    margin-top: 3px;
    font-size: 12px;
    color: #666;
  }
}
span {
  font-size: 12px;
}
</style>