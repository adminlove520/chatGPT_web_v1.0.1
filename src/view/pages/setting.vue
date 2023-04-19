<template>
  <div class="setting">
    <el-container>
      <el-header>
        <transition name="el-zoom-in-top">
          <div v-show="show" class="transition-box">
            <h3>隐侠AI-Web</h3>
          </div>
        </transition>
      </el-header>
      <el-main>
        <transition name="el-zoom-in-top">
          <div v-show="show" class="transition-box">
            <span>
              东方隐侠团队，专注于网络安全基础能力研究，热衷于红蓝对抗、企业安全建设等知识的分享与输出。
              现有成员30+位，包含多位护网红队TOP3选手、国内大型安全厂商专家、业内元老等，
              技术研究方向涵盖红蓝对抗、安全运营、数据安全、AI安全、二进制分析、移动安全等领域。。
            </span>
          </div>
        </transition>
      </el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      show: false,
    };
  },
  mounted() {
    this.show = true;
  },
};
</script>

<style>
  .transition-box {
    text-align: center;
    margin-top: 5%;
    color: #F2F6FC;
    font-size: 30px;
  }
  h1 {
    color: aliceblue;
    font-size: 80px;
  }
  a {
    text-decoration: none;
    color: #67C23A;
  }
</style>
