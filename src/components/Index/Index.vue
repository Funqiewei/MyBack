<template>
  <el-container class="index-container">
    <el-header>
      <div>
        <!-- 用~@图不会裂好奇怪 -->
        <!-- 怎么解决vue动态设置img的src不生效的问题 -->
        <!-- 或者因为动态添加src被当做静态资源处理了，没有进行编译，所以要加上require。
<img class="logo" :src="require("./../assets/images/logo.png")" alt="公司logo"> -->
        <img
          src="~@/assets/kylogo2.png"
          @click="click_logo2"
          width="40%"
          height="50%"
          style="vertical-align: text-bottom"
        /> 
        <div class="text">
        <!-- <a @click="click_test">test</a> -->
        <a @click="click_index">首页</a>
        <a @click="click_help">支持与帮助 </a>
        <a @click="click_console">控制台</a>
        </div> 
      </div>
      
    </el-header>
    <el-main>
      <!-- 路由占位符 -->
      <router-view> </router-view>
      <!-- <div class="footer">
          <div class="footer_left">
            <p>咨询电话:0575-82001777</p>
            <p></p>
            <p>院长书记信箱:</p>
            <p>ky@zstu.edu.cn </p>
          </div>
          <div class="footer_center">
            <p>浙江理工大学科技与艺术学院</p>
            <p>学院地址：</p>
            <p>杭州湾上虞经济技术开发区康阳大道58号</p>
          </div>
          <div class="footer_right">
            <p>邮编:312369</p>
            <p></p>
            <p>传真:0575-82978000</p>
            <p> Copyright(c)2021
            </p>
            
          </div>
        </div> -->
        <div class="sch_motto">—厚德致远·博学敦行 —</div>
    </el-main>  
    </div>

  </el-container>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {
    click_logo2() {
      window.location.href = "http://www.ky.zstu.edu.cn/";
    },
    click_doc() {
      this.$router.push("/document");
    },
    click_index() {
      this.$router.push("/Index");
    },
    click_help() {
      this.$router.push("/Help");
    },
    click_console() {
      this.$router.push("/login");
    },
    click_test() {
      this.$router.push("/test");
    },
  },
};
</script>


<style lang="less" scoped>
.index-container {
  height: 100%;
  padding-left: 0px;
  padding-right: 0px;
  padding-top: 0px;
  padding-bottom: 0px;
}
.el-header {
  background-color: #ffffff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 10px;
  height: 10%;
  font-size: 15px;
  vertical-align: middle;
  > div {
    display: flex;
    align-items: center;
    span {
      margin-left: 10px;
    }
  }
}
.text {
  position: absolute;
  right: 20px;
}
// .title {
//   padding-top: 20px;
//   font-weight: bold;
//   font-size: 2rem;
// }
// .title2 {
//   margin-top: 15px;
//   font-size: 1rem;
// }
// .main_container {
//   width: 100%;
//   margin-right: auto;
//   margin-left: auto;
//   background-color: #000;
//   text-align: center;
//   color: #ffffff;
// }
.el-main {
  background-color: #ffffff;
  width: 100%;
  padding-left: 0px;
  padding-right: 0px;
  padding-top: 0px;
  padding-bottom: 0px;
  line-height: 60px;
}
.footer_left {
  text-align: center;
  width: 100%;
}
.footer_center {
  text-align: center;
  width: 100%;
}
.footer_right {
  text-align: center;
  width: 100%;
}
.footer-container {
  background: #ebebeb;
  height: 200px;
  width: 100%;
  margin: 0;
}

.footer {
  background-color: #fff;
  width: 100%;
  font-size: 14px;
  line-height: 30px;
  border-top: solid #cccc;
  display: flex;
}
.sch_motto {
  text-align: center;
  border-top: solid #cccc;
  font-size: 16px;
  font-weight: 900;
  line-height: 57px;
  color: #9c9c9c;
  display: block;
}
a {
  margin-left: 25px;
  width: 150;
}
a:hover {
  font-weight: bold;
  border-bottom: 2px solid;
}
</style>