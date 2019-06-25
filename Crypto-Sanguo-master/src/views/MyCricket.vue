<template>
  <div class="qq-list">
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
    <div class="qq-item">
      <img src="../assets/img/qq1.png">
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    showResult: false
  }),

  computed: {},

  created() {},

  watch: {},

  methods: {
    getQQ() {
      this.showResult = true;
    }
  }
};
</script>
 <style scoped>
.qq-list {
  width: 720px !important;
  margin: 0 auto;
  padding-bottom: 60px;
}
.qq-item {
  width: 200px;
  height: 200px;
  display: inline-block;
  margin-top: 60px;
  background-image: url("../assets/img/p1.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
  cursor: pointer;
}
.selectResultBox {
  text-align: center;
}
.selectResultTitle {
  margin-top: 60px;
  font-size: 20px;
  font-weight: bold;
  color: white;
}
.selectBtn {
  width: 250px;
  height: 250px;
  margin: 0 auto;
  margin-top: 100px;
  background-image: url("../assets/img/getBtn.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
  cursor: pointer;
}
.selectResult {
  width: 250px;
  height: 250px;
  margin: 0 auto;
  margin-top: 60px;
  background-image: url("../assets/img/p1.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
  cursor: pointer;
}
</style>
