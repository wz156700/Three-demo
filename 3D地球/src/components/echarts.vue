<template>
  <div style="">
    <div style="
        position: absolute;
        left: 640px;
        top: 940px;
        font-size: 16px;
        color: #33bbbb;
        padding: 10px 20px;
        background: rgba(0, 0, 0, 0.06);
        width: 230px;
        border-radius: 10px;
      ">
      <div style="color:#ffffff;border-bottom: #004444 solid 1px;padding: 10px 20px;">人次</div>
      <!-- <div style="font-size: 16px; color: #eee; padding: 2px 4px;margin-left:193px;">人口</div> -->
      <div id="all" class="number" style="letter-spacing: 16px; font-size: 64px; color: #00ffff">
        68650
      </div>
      
    </div>

        <div style="
        position: absolute;
        left: 1060px;
        top: 940px;
        font-size: 16px;
        color: #33bbbb;
        padding: 10px 20px;
        background: rgba(0, 0, 0, 0.06);
        width: 230px;

        border-radius: 10px;
      ">
      <div style="color:#ffffff;border-bottom: #004444 solid 1px;padding: 10px 20px;">架次</div>
      <!-- <div style="font-size: 16px; color: #eee; padding: 2px 4px;margin-left:193px;">人口</div> -->
      <div id="all" class="number" style="letter-spacing: 16px; font-size: 64px; color: #00ffff">
        33351
      </div>
      
    </div>

    <div style="
        position: absolute;
        left: 1490px;
        top: 90px;
        background: rgba(0, 0, 0, 0.06);
        border-radius: 10px;
        padding: 20px 10px;
        z-index: 10;
      ">
      <div style="color:#ffffff;padding: 10px 20px;width: 360px;">起飞架次(每小时)</div>
      <div id="echarts1" style="width: 400px; height: 200px"></div>
    </div>

    <div style="
        position: absolute;
        left: 1490px;
        top: 395px;
        background: rgba(0, 0, 0, 0.06);
        border-radius: 10px;
        padding: 0px 10px;
        z-index: 10;
      ">
      <!-- <div style="color:#ffffff;padding: 10px 20px;width: 360px;text-align: center;">计划完成度</div> -->
      <div id="echarts2" style="width: 400px; height: 360px"></div>
    </div>

    <div style="
        position: absolute;
        left: 1490px;
        top: 780px;
        background: rgba(0, 0, 0, 0.06);
        border-radius: 10px;
        padding: 10px 20px;
        z-index: 10;
      ">
      <!-- text-align: center; -->
            <div style="color:#ffffff;padding: 10px 20px;width: 360px;">计划完成度</div>

      <div id="echarts3" style="width: 400px;; height: 240px"></div>
    </div>

    <div style="
        position: absolute;
        left: 10px;
        top: 90px;
        background: rgba(0, 0, 0, 0.06);
        border-radius: 10px;
        padding: 20px 10px;
        z-index: 10;
      ">
      <div id="echarts4" style="width: 400px;; height: 240px"></div>
    </div>

    <div style="
        position: absolute;
        left: 10px;
        top: 395px;
        background: rgba(0, 0, 0, 0.06);
        border-radius: 10px;
        padding: 0px 10px;
        z-index: 10;
      ">
      <div id="echarts5" style="width: 400px;; height: 360px"></div>
    </div>

    <div style="
        position: absolute;
        left: 10px;
        top: 780px;
        background: rgba(0, 0, 0, 0.06);
        border-radius: 10px;
        padding: 10px 20px;
        z-index: 10;
      ">
      <div id="echarts6" style="width:380px; height: 270px"></div>
    </div>
    <!--定义画布  background: rgba(255,255,255,0.17)-->
    <!-- <div style="position: absolute;left: 10px;top: 300px;background: rgba(0, 0, 0, 0.09);padding:20px 10px;border-radius: 10px;">

    <canvas id="canvas" width="100px" height="480px" style="">
    </canvas>
  </div> -->

    <!-- <div
    style="position: absolute;left:1530px;top:160px;background:rgba(0,0,0,0.15);border-radius: 10px;padding: 20px 10px;z-index:10;">
    <div id="echarts3" style="width: 400px;height: 240px;"></div>
  </div> -->

    <!-- <div
    style="position: absolute;left:1530px;top:160px;background:rgba(0,0,0,0.15);border-radius: 10px;padding: 20px 10px;z-index:10;">
    <div id="echarts3" style="width: 400px;height: 240px;"></div>
  </div> -->

    <!-- <div
    style="position: absolute;left:1530px;top:600px;background:rgba(0,0,0,0.15);border-radius: 10px;padding: 0px 10px;z-index:10;">
    <div id="echarts4" style="width: 400px;height: 360px;"></div>
  </div> -->
  </div>
</template>

<script>
import line from "./echarts/line.js";
import ring from "./echarts/ring.js";
// import radar from "./echarts/radar.js";
// import meter from "./echarts/meter.js";
import shuizhu from "./echarts/shuizhu.js";
import shuzhu from "./echarts/shuzhu.js";
import water from "./echarts/water.js";
import linedan from "./echarts/linedan.js";
export default {
  name: "echarts",
  mounted: function () {
    linedan("echarts1");
    shuzhu("echarts2");

    water("echarts3");

    line("echarts4");
    ring("echarts5");

    shuizhu("echarts6");
    // water("echarts4");



  },
};
</script>


<style scoped>
/* .container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-content: space-between;
} */

/* .item {
  background: #ffffff;
  width: 290px;
  height: 360px;
} */


</style>
