 <template>
  <div class="width:20%">
    <div class="main_container">
      <div class="title">开启校园预约新生活</div>
      <div class="title2">物联网项目开发</div>
      <div>
        <img src="~@/assets/IndexBgpic.png" alt="" width="50%" />
      </div>
    </div>

    <div class="Indexpic">
      <div class="intro">
        <h1>操作简单</h1>
          <p>
            &nbsp &nbsp &nbsp
            &nbsp为校园物联网生活赋能，提供通用的物联网设备连接、设备管理、IoT
            边缘及数据流转能力，赋能产业应用。
            为物联网平台提供更基础中台能力，并整合连接、设备管理、边缘计算和规则引擎，提供物联网平台核心功能集合。
          </p>
      </div>
      <div>
        <img src="~@/assets/IndexBgpic2.png" alt="" width="100%" height="100%"/>
      </div>
      
    </div>

    <div class="Indexpic">
      <div class="intro">
        <h1>协同服务</h1>
          <p>
            &nbsp &nbsp &nbsp
            &nbsp物联网应用的标配数据库，高效支撑物联网时序数据的存储和分析，特别适用于物联网设备监控和数据分析，以及互联网业务监控场景。
            将云计算能力延伸至边缘，支持设备接入等能力，提供实时可靠服务，实现边缘自治，边云协同。
          </p>
      </div>
      <div>
        <img src="~@/assets/IndexBgpic3.png" alt="" width="100%" height="100%" />
      </div>
      
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
.title {
  padding-top: 20px;
  font-weight: bold;
  font-size: 2rem;
}
.title2 {
  margin-top: 15px;
  font-size: 1rem;
}
.main_container {
  width: 100%;
  margin-right: auto;
  margin-left: auto;
  background-color: #000;
  text-align: center;
  color: #ffffff;
}
.intro {
  margin-left: 5%;
  margin-right: 5%;
  margin-top: 2%;
  > p {
    font-size:  1rem;
    color: #231815;
    font-weight: 300;
    display: flex;
  }
}
.Indexpic {
  display: flex;
   margin-left: 5%;
  margin-right: 5%;
  margin-top: 2%;
  margin-bottom: 2%;
  >div{
    > img {
    border-radius: 15px;
    display: flex;

  }
  }
}
</style>