<template>
  <div class="news">
    <div class="news-main-pos">
      <div class="lunbo">
        <div class="focus fl">
          <a href="javascript:;" @click="gotoPage(prevIndex)" class="arrow-l"
            >&lt;</a
          >
          <a href="javascript:;" @click="gotoPage(nextIndex)" class="arrow-r"
            >&gt;</a
          >
          <img :src="dataList[currentIndex]" />
        </div>
      </div>
      <div class="dongtai">
        <div>
          <span><i class="bi bi-newspaper"></i>&nbsp;新闻动态</span>
          <span style="float: right"><a href="">更多》</a></span>
        </div>
        <div class="dtimg">
          <img src="../../static/assets/images/news-pc.png" alt="" />
          <div>
            牢记使命跟党走<br />楷模精神育新人<br />&nbsp;&nbsp;&nbsp;&nbsp;（天津日报）
          </div>
        </div>
        <div class="dtnews">
          <ul>
            <li>
              <a href=""
                ><i class="bi bi-journal-text"></i> <span>妇女节快乐</span></a
              >
            </li>
            <li>
              <a href=""
                ><i class="bi bi-journal-text"></i>
                <span>“你好天津”展示小视频</span></a
              >
            </li>
            <li>
              <a href=""
                ><i class="bi bi-journal-text"></i>
                <span>周邓馆迎来参观高峰（今晚报）</span></a
              >
            </li>
            <li>
              <a href=""
                ><i class="bi bi-journal-text"></i>
                <span>纪念周恩来通知诞辰124周年</span></a
              >
            </li>
            <li>
              <a href=""
                ><i class="bi bi-journal-text"></i>
                <span>周恩来邓颖超纪念馆职工纪念周恩来通知诞辰</span></a
              >
            </li>
          </ul>
        </div>
      </div>
      <div class="gonggao">
        <div>
          <span><i class="bi bi-newspaper"></i>&nbsp;最新公告</span>
          <span style="float: right"><a href="">更多》</a></span>
        </div>
        <ul>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i>
              <span style="font-weight: 800; color: red">开馆公告</span></a
            >
          </li>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i> <span>闭馆公告</span></a
            >
          </li>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i>
              <span>周恩来邓颖超纪念馆2022年元旦放假开放公告</span></a
            >
          </li>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i> <span>临时展览展讯</span></a
            >
          </li>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i>
              <span>周恩来邓颖超纪念馆2020年度部门决算和“三公”经费决算</span></a
            >
          </li>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i>
              <span>周恩来邓颖超纪念馆主题展厅对外开放公告</span></a
            >
          </li>
          <li>
            <a href=""
              ><i class="bi bi-journal-text"></i>
              <span>“光辉的历程--中共共产党百年图片展”展览公告</span></a
            >
          </li>
        </ul>
      </div>
      <div class="jianjie">
        <div class="jiben">基本简介</div>
        <div class="jcontent">
          <p>
            周恩来邓颖超纪念馆坐落在风光旖旎、景色怡人的水上公园风景区，占地70000平方米，建筑面积13000平方米，建于1998年2月28日周恩来诞辰百年纪念日前夕。馆内藏品丰富，文物价值弥足珍贵。
          </p>
        </div>
        <img src="../../static/assets/images/jianjie.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dataList: [
        "../../static/assets/images/xdd.jpg",
        "../../static/assets/images/airplane.jpg",
        "../../static/assets/images/car.jpg",
        "../../static/assets/images/chain.jpg",
      ],

      // 默认显示图片
      currentIndex: 0,
      // 定时器
      timer: null,
    };
  },
  methods: {
    gotoPage(index) {
      this.currentIndex = index;
    },
    // 定时器
    runInv() {
      this.timer = setInterval(() => {
        this.gotoPage(this.nextIndex);
      }, 1000);
    },
  },
  computed: {
    // 上一张
    prevIndex() {
      if (this.currentIndex === 0) {
        return this.dataList.length - 1;
      } else {
        return this.currentIndex - 1;
      }
    },
    // 下一张
    nextIndex() {
      if (this.currentIndex === this.dataList.length - 1) {
        return 0;
      } else {
        return this.currentIndex + 1;
      }
    },
  },
};
</script>

<style scoped>
a {
  color: #000;
  text-transform: capitalize;
}
.news {
  position: relative;
  width: 100%;
  height: 930px;
  background: url(../../static/assets/images/news-bc.png) no-repeat;
  background-position: 0 35%;
  background-size: cover;
}
.news-main-pos {
  width: 78%;
  height: 930px;
  left: 50%;
  transform: translateX(-49%);
  position: absolute;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  flex-direction: row;
}
/* .news-main {
  width: 100%;
  height: 920px;
  transform: translate(-49%, -50%);
} */
/* 新闻动态 */
.dongtai {
  height: 520px;
  width: 40%;
}
.dongtai div:nth-child(1) {
  height: 40px;
  line-height: 40px;
  border-bottom: 3px solid red;
  margin-bottom: 5px;
}
.dongtai span:first-child {
  font-weight: 600px;
  font-size: 25px;
}
.dtimg {
  position: relative;
  width: 60%;
  height: 160px;
}
.dongtai .dtimg img {
  width: 100%;
  height: 100%;
}
.dongtai .dtimg div {
  width: 70%;
  position: absolute;
  display: inline-block;
  color: #b32521;
  font-weight: 600;
  font-size: 25px;
  margin-left: 30px;
  margin-top: 10px;
}
.dongtai .dtnews ul li {
  height: 58px;
  line-height: 58px;
}
ul li {
  padding-left: 5px;
  font-size: 22px;
  border-bottom: 2px dashed #c5c5c5;
}
ul li i {
  color: red;
}
/* 最新公告 */
.gonggao {
  height: 400px;
  width: 45%;
  margin-right: 35px;
}
.gonggao div:nth-child(1) {
  height: 40px;
  line-height: 40px;
  border-bottom: 3px solid red;
}
.gonggao span:first-child {
  font-weight: 600px;
  font-size: 25px;
}
.gonggao ul li {
  height: 50px;
  line-height: 50px;
}
/* 基本简介 */
.jianjie {
  height: 400px;
  width: 45%;
  position: relative;
}
.jianjie img {
  height: 400px;
  width: 100%;
}
.jiben {
  position: absolute;
  top: 30px;
  width: 140px;
  height: 55px;
  line-height: 55px;
  background-color: #9f0000;
  color: #ffff;
  font-size: 30px;
  padding-left: 10px;
}
.jcontent {
  width: 100%;
  height: 90px;
  position: absolute;
  bottom: 0;
  color: #ffff;
  background: url(../../static/assets/images/jianjiebc.png) no-repeat;
  text-indent: 2em;
  font-size: 20px;
}
/* 轮播图部分 */
* {
  margin: 0;
  padding: 0;
}
.lunbo {
  height: 500px;
  width: 50%;
  margin-right: 30px;
}
.focus img {
  margin-top: 5px;
  width: 100%;
  height: 499px;
  display: block;
}
.focus {
  position: relative;
  overflow: hidden;
  max-width: 1200px;
  margin: 0 auto;
}
.fl {
  float: left;
}
.arrow-l,
.arrow-r {
  display: block;
  position: absolute;
  top: 50%;
  margin-top: -20px;
  width: 30px;
  height: 80px;
  background: rgba(0, 0, 0, 0.2);
  text-align: center;
  line-height: 80px;
  color: #fff;
  font-family: "icomoon";
  font-size: 18px;
  font-weight: 600;
  z-index: 2;
}

.arrow-r {
  right: 0;
}
</style>

