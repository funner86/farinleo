<template>
  <!-- Header Area Starts -->
  <header class="header-area single-page">
    <div class="header-top">
      <div class="row top-background">
        <div class="ht-background">
          <div class="main-menu2">
            <ul>
              <li>
                <img
                  src="../../static/assets/images/user.png"
                  alt=""
                  width="40px"
                  height="35px"
                />
              </li>
              <li>
                <div style="float: left">
                  <form action=""><input type="text" /></form>
                </div>
                <div class="imgflex">
                  <img
                    src="../../static/assets/images/search.png"
                    alt=""
                    width="35px"
                    height="25px"
                  />
                </div>
              </li>
              <li style="padding-top: 5px">
                <a href="" style="color: #e6d799">中文|ENGLISH|日本語</a>
              </li>
              <li style="padding-top: 5px">您好，欢迎光临周恩来邓颖超纪念馆</li>
            </ul>
          </div>
          <div class="col-lg-10 top-container">
            <div class="main-menu main-menu-light">
              <ul>
                <li class="active">
                  <router-link to="/">首页</router-link>
                </li>
                <li><router-link to="/about">概况</router-link></li>
                <li><router-link to="/category">咨询</router-link></li>
                <li>
                  <a href="#">陈列展览</a>
                  <!-- <ul class="sub-menu">
                      <li><router-link to="/blog">Blog Home</router-link></li>
                      <li>
                        <router-link to="/blogDetails"
                          >Blog Details</router-link
                        >
                      </li>
                    </ul> -->
                </li>
                <li><router-link to="/contact">文物鉴赏</router-link></li>
                <li>
                  <a href="#">教育园地</a>
                  <!-- <ul class="sub-menu">
                      <li>
                        <router-link to="/jobSearch">Job Search</router-link>
                      </li>
                      <li>
                        <router-link to="/jobSingle">Job Single</router-link>
                      </li>
                      <li>
                        <router-link to="/pricingPlan"
                          >Pricing Plan</router-link
                        >
                      </li>
                      <li>
                        <router-link to="/elements">Elements</router-link>
                      </li>
                    </ul> -->
                </li>
                <li><router-link to="/about">学术研究</router-link></li>
                <li><router-link to="/category">基地活动</router-link></li>
                <li><router-link to="/about">信息互动</router-link></li>
                <li><router-link to="/category">服务指南</router-link></li>
                <!-- <li class="menu-btn">
                    <a href="#" class="login">log in</a>
                    <a href="#" class="template-btn">sign up</a>
                  </li> -->
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="page-title">
      <div>
        场馆开放时间<br />
        <span style="font-size: 50px; color: #edf3fd"> 9:00-16:00</span>
      </div>
      <div>
        <span style="font-size: 40px; color: #edf3fd">15:30</span>
        <span style="font-size: 20px; color: #edf3fd">
          点后停止入馆 周一闭馆，法定节假日除外
        </span>
      </div>
      <div>
        联系电话<br />
        <span style="font-size: 30px; color: #edf3fd">
          022-23592257<br />
          022-81110903
        </span>
      </div>
      <div>
        <p style="margin: 100px 0 0 10px">参观预约</p>
      </div>
      <div>
        <p style="margin: 100px 0 0 10px">交通路线</p>
      </div>
      <div></div>
      <div></div>
    </div>
  </header>
  <!-- Header Area End -->
</template>

<script>
export default {};
</script>

<style>
.top-background .ht-background {
  width: 3000px;
  margin-left: 15px;
  height: 220px;
  background: url(../../static/assets/images/topbc.png) no-repeat;
  background-size: 100% 200px;
}
.top-background .top-container {
  position: relative;
  top: 42px;
  float: right;
  display: flex;
}
</style>
