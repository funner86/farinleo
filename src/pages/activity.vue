<template>
  <div class="acitivity">
    <div class="col-appre">
      <div class="col-text">
        <div class="ctext">
          <span>典藏鉴赏</span>
          <img src="../../static/assets/images/diancang.png" alt="" />
        </div>
      </div>
    </div>
    <div class="base-act">
      <div class="base-top">
        <span>基地活动</span>
        <span style="float: right"
          ><a href="" style="color: #fff">更多 》</a></span
        >
      </div>
      <div class="base-bot">
        <ul>
          <li><a href="">2021年共建基地与周邓班</a></li>
          <li><a href="">2020年共建基地与周邓班</a></li>
          <li><a href="">2019年共建基地与周邓班</a></li>
          <li><a href="">2018年共建基地与周邓班</a></li>
          <li><a href="">2017年共建基地与周邓班</a></li>
          <li><a href="">2016年共建基地与周邓班</a></li>
          <li><a href="">2015年共建基地与周邓班</a></li>
          <li><a href="">2014年共建基地与周邓班</a></li>
          <li><a href="">2013年共建基地与周邓班</a></li>
          <li><a href="">2012年共建基地与周邓班</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
/* 主体 */
.acitivity {
  width: 100%;
  height: 930px;
  display: flex;
  align-items: center;
}
/* 典藏鉴赏部分 */
.col-appre {
  height: 90%;
  width: 30%;
  margin-left: 40px;
  background: url(../../static/assets/images/ZD_03.png) no-repeat center;
  background-size: 100% 850px;
  background-position: -20px center;
}
.ctext {
  position: relative;
  height: 837px;
  width: 100%;
}
.ctext span {
  position: absolute;
  color: #fff;
  font-size: 60px;
  font-weight: 800;
  writing-mode: vertical-lr;
  top: 15%;
  left: 42%;
}
.ctext img {
  position: absolute;
  top: 52%;
  left: 10%;
  width: 70%;
}
/* 基地活动部分 */
.base-act {
  margin-left: 60px;
  height: 90%;
  width: 64%;
  background: url(../../static/assets/images/act-bc.png) no-repeat center;
}
.base-top {
  width: 100%;
  height: 17%;
  line-height: 100px;
  padding: 15px;
  border-bottom: 5px solid #fff;
}

.base-top span {
  font-size: 50px;
  font-weight: 800;
  color: #fff;
  margin-left: 24px;
}
.base-top a {
  font-size: 20px;
  font-weight: 800;
  color: #fff;
}
.base-bot {
  width: 100%;
  height: 83%;
}
.base-bot ul {
  width: 1200px;
  margin: auto;
}
.base-bot li {
  display: block;
  width: 590px;
  float: left;
  margin-top: 60px;
  padding-left: 40px;
  font-size: 40px;
  font-weight: 600;
  color: #fff;
  letter-spacing: 4px;
}
.base-bot a {
  color: #fff;
}
</style>