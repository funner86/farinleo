<template>
  <div class="chenlie">
    <div class="CL">
      <div class="ZLL"></div>
      <div class="ZLR">
        <div class="ZLR-TOP"></div>
        <div class="ZLR-BOT"></div>
      </div>
    </div>
    <div class="CR">
      <a href="" class="ACres">
        <div><span>学术研究</span></div></a
      >
      <a href="" class="EDUgen">
        <div><span>教育园地</span></div></a
      >
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.chenlie {
  width: 100%;
  height: 900px;
  border: 3px solid yellow;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
/* .dingwei {
  margin: 50px auto;

  width: 1900px;
} */
/* 陈列展览 */
.CL {
  display: flex;
  border: 3px solid red;
  margin-left: 20px;
  width: 1100px;
  height: 830px;
}
.CL .ZLL {
  width: 10%;
  height: 100%;
  border-right: 1px solid red;
}
.CL .ZLR {
  width: 90%;
  height: 825px;
  display: flex;
  flex-direction: column;
}
.CL .ZLR .ZLR-TOP {
  width: 100%;
  height: 600px;
  border: 2px solid green;
  background-color: pink;
}
.CL .ZLR .ZLR-BOT {
  width: 100%;
  height: 225px;
  border: 2px solid black;
  background-color: yellow;
}
/* 学术研究 */
.CR {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 830px;
  width: 700px;
  margin-right: 20px;
}
.ACres {
  width: 95%;
  height: 400px;
  background-color: pink;
  margin-bottom: 20px;
  background: url(../../static/assets/images/acres-bc.png) no-repeat center;
  background-size: 716px 400px;
}
.ACres span {
  color: #fff;
  font-size: 50px;
  font-weight: 600;
  letter-spacing: 4px;
  margin-top: 30px;
  margin-right: 35px;
  float: right;
}
/* 教育园地 */
.EDUgen {
  width: 95%;
  height: 400px;
  background: url(../../static/assets/images/edu-bc.png) no-repeat center;
  background-size: 700px 400px;
}
.EDUgen span {
  color: #fff;
  font-size: 50px;
  font-weight: 600;
  letter-spacing: 4px;
  margin-top: 30px;
  margin-left: 35px;
  float: left;
}
</style>