<template>
  <div class="home">
    <top-view/>
    <sales-view/>
    <bottom-view/>
    <map-view/>
  </div>
</template>

<script>
import TopView from "@/components/TopView/TopView";
import SalesView from "@/components/SalesView/SalesView";
import BottomView from "@/components/BottomView/BottomView";
import MapView from "@/components/MapView/MapView";
export default {
  name: 'Home',
  components: {MapView, BottomView, SalesView, TopView},
}
</script>

<style lang="scss">
.home{
  width: 100%;
  height: 100%;
  padding: 20px;
  background: #eee;
}
</style>
