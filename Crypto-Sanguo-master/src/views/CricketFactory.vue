<template>
  <div>
    <div v-if="!showResult" @click="getQQ" class="selectBtn"></div>
    <div v-if="showResult" class="selectResultBox">
      <h1 class="selectResultTitle">恭喜! 您获得了一只蛐蛐～</h1>
      <div class="selectResult">
        <img src="../assets/img/qq1.png">
      </div>
    </div>
  </div>
</template>

<script>
import { getPackageSize } from "@/api";

export default {
  data: () => ({
    showResult: false,
    packageSize: 0
  }),

  computed: {},

  created() {
    this.refresh();
  },

  watch: {},

  methods: {
    getQQ() {
      this.showResult = true;
    },
    async refresh() {
      this.packageSize = await getPackageSize();
      alert(this.packageSize);
    }
  }
};
</script>
 <style scoped>
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
