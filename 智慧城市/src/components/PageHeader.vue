<template>
    <div style="display: flex; flex-direction: row; align-items: center">
      <!-- background:rgba(255, 0, 0, 0.0);用来辅助测试观察布局效果 -->
      <div
        style="
          background: rgba(255, 0, 0, 0);
          color: #ffffff;
          width: 50px;
          height: 50px;
        "
      >
        <img src="../assets/UI/城市.png" alt="" style="height: 100%" />
      </div>
      <div
        style="
          background: rgba(255, 0, 0, 0);
          color: #ffffff;
          width: 245px;
          height: 20px;
          margin-left: 20px;
        "
      >
        智慧城市
      </div>
      <!-- flex嵌套flex布局 -->
      <div
        style="
          display: flex;
          flex-direction: row;
          align-items: center;
          background: rgba(0, 0, 0, 0.25);
          border-radius: 40px;
          padding: 10px 20px;
          margin-left: 1370px;
        "
      >
        <div
          style="
            background: rgba(255, 0, 0, 0);
            color: #ffffff;
            width: 32px;
            height: 32px;
          "
        >
          <img src="../assets/UI/多云.png" alt="" style="height: 100%" />
        </div>
        <div
          style="
            height: 30px;
            width: 1px;
            background: rgba(0, 160, 200, 0.4);
            margin-left: 10px;
          "
        ></div>
        <div
          style="
            background: rgba(255, 0, 0, 0);
            color: #ffffff;
            margin-left: 10px;
            height: 28px;
          "
        >
          <img src="../assets/UI/PM2.5.png" alt="" style="height: 28px" />
        </div>

        <div
          style="
            background: rgba(255, 0, 0, 0);
            color: #ffffff;
            margin-left: 10px;
          "
        >
          57.0
        </div>
        <div
          style="
            height: 30px;
            width: 1px;
            background: rgba(0, 160, 200, 0.4);
            margin-left: 10px;
          "
        ></div>
        <div
          style="
            background: rgba(255, 0, 0, 0);
            color: #ffffff;
            margin-left: 0px;
            height: 32px;
          "
        >
          <img src="../assets/UI/温度.png" alt="" style="height: 32px" />
        </div>
        <div
          style="
            background: rgba(255, 0, 0, 0);
            color: #ffffff;
            margin-left: 0px;
          "
        >
          36.5
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: "PageHeader",
};
</script>


<style scoped>
</style>
