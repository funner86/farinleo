<template>
  <footer>
    <div class="footer">
      <div class="wenchuang">
        <div class="wphoto">
          <div>
            <a href=""
              ><img src="../../static/assets/images/w2.png" alt="" />
              <div class="wtext">瞻仰未来金箔画</div>
            </a>
          </div>
          <div>
            <a href=""
              ><img src="../../static/assets/images/w3.png" alt="" />
              <div class="wtext">周恩来百年书目图典</div>
            </a>
          </div>
          <div>
            <a href=""
              ><img src="../../static/assets/images/w4.png" alt="" />
              <div class="wtext">建党90周年纪念邮册</div>
            </a>
          </div>
          <div>
            <a href=""
              ><img src="../../static/assets/images/w1.png" alt="" />
              <div class="wtext">伟人铜盘</div>
            </a>
          </div>
          <div>
            <a href=""
              ><img src="../../static/assets/images/w5.png" alt="" />
              <div class="wtext">五四邮折</div>
            </a>
          </div>
          <div>
            <button>更<br />多<br />&nbsp;》</button>
          </div>
        </div>
      </div>
      <div class="footer-area footer-content">
        <div class="xcontent">
          <div>
            <img src="../../static/assets/images/footer-zd.png" alt="" />
          </div>
          <div>
            <img src="../../static/assets/images/chat.png" alt="" />
          </div>
          <div>
            <div style="margin-bottom: 50px; width: 310px">
              <a href="">百度百科</a><a href="">免责声明</a
              ><a href="">关于我们</a>
            </div>
            <div style="display: inline-block; width: 366px">
              <span>版权所有：周恩来邓颖超纪念馆</span>
              <span>地址：天津市南开区水上公园西路9号</span>
              <span>电话：033-23592257 81110903</span>
            </div>
            <div style="display: inline-block; width: 430px">
              <span>津ICP备19011388号-1</span>
              <span>邮编:300074</span>
              <span>电子邮件：ZHOUDENG1@MZHOUDENG.COM</span>
            </div>
            <div>
              <span
                >周恩来邓颖超纪念馆微博：HTTP://WEIBO.COM/P/1001065700080604</span
              >
            </div>
          </div>
          <div>
            <div class="zztj">
              <img src="../../static/assets/images/zztj.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
  <!-- Footer Area End -->
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  display: flex;
  flex-direction: column;
}
.footer .wenchuang {
  height: 450px;
  background: url(../../static/assets/images/wenchuang.png) no-repeat center;
  background-size: 100% 450px;
}

.footer .wenchuang .wphoto {
  display: flex;
  position: relative;
  justify-content: space-between;
  top: 102px;
}
.footer .wenchuang .wphoto div {
  height: 280px;
}
.footer .wenchuang div img {
  margin-top: 20px;
  height: 200px;
  width: 100%;
}
.footer .wenchuang .wphoto > div:nth-child(2) img {
  margin-left: 50%;
  transform: translateX(-50%);
}

.footer .wenchuang .wphoto div > button {
  height: 99%;
  background-color: rgba(255, 254, 254, 0.1);
  color: #fffefe;
  font-size: 20px;
  font-weight: 600;
}
.footer .wenchuang .wphoto .wtext {
  color: #fffefe;
  text-align: center;
  margin-top: 15px;
  font-size: 25px;
}

/* 最底部 */
.footer .footer-content .xcontent {
  display: flex;
  justify-content: space-between;
}
.footer .footer-content .xcontent > div:nth-child(1) {
  position: relative;
  width: 350px;
  height: 400px;
  top: 50px;
}
.footer .footer-content .xcontent > div:nth-child(1) > img {
  margin-top: 50%;
  transform: translateY(-40%);
  width: 325px;
}
.footer .footer-content .xcontent > div:nth-child(2) {
  position: relative;
  width: 350px;
  height: 400px;
  top: 50px;
  margin-right: 30px;
}
.footer .footer-content .xcontent > div:nth-child(2) > img {
  margin-top: 50%;
  transform: translateY(-40%);
  width: 350px;
}
.footer .footer-content .xcontent > div:nth-child(3) {
  position: relative;
  height: 400px;
  top: 100px;
  overflow: hidden;
}
.footer .footer-content .xcontent > div:nth-child(3) span {
  font-size: 18px;
  margin-right: 30px;
  margin-bottom: 40px;
  display: block;
}
.xcontent > div:nth-child(3) > div a {
  margin-right: 35px;
}
.footer .footer-content .xcontent > div:nth-child(4) {
  position: relative;
  width: 300px;
  top: 115px;
}
.zztj > img {
  position: absolute;
  width: 300px;
  height: 325px;
}
</style>
