<template>
  <div>
    <div class="leader">
      <LeaderComponent></LeaderComponent>
    </div>
    <div class="content">
      <div class="paper">
        <div class="box">
          <h1>简历</h1>
          <div class="p-head">
            <div class="p-h-left">
              <p>
                <span>前端开发</span>正式工作或实习
              </p>
            </div>
            <div class="p-h-center">
              <p>喜欢并擅长协调、经营的工作。关注用户的内容偏好，有一定的数据分析能力。喜欢新技术、新产品，对互联网产品的运营有浓厚的兴趣和热情。坚信好的互联网产品必将营造更美好的生活。</p>
            </div>
            <div class="p-h-photo">
              <img src="./img/wechat.jpg" alt="头像">
            </div>
          </div>
          <!-- 简历内容 -->
          <div class="p-content">
            <!-- 简历左边 -->
            <div class="p-c-left">
              <!-- table1 -->
              <table>
                <tr>
                  <th>个人信息</th>
                </tr>
                <tr>
                  <td>姓名 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 陈国华</td>
                </tr>
                <tr>
                  <td>生日 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;1998.08.29</td>
                </tr>
                <tr>
                  <td>所在地&nbsp; &nbsp; &nbsp; &nbsp;广东省江门市台山市</td>
                </tr>
                <tr>
                  <td>Email&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;2464231008@qq.com</td>
                </tr>
                <tr>
                  <td>手机 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;13059247423</td>
                </tr>
                <tr>
                  <td>QQ &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;2464231008</td>
                </tr>
              </table>
              <!-- table2 -->
              <table class="t2">
                <tr>
                  <th>教育背景</th>
                </tr>
                <tr>
                  <td>
                    <span class="orange">广东理工学院</span>
                  </td>
                </tr>
                <tr>
                  <td>信息工程系 &nbsp; &nbsp;软件技术专业</td>
                </tr>
                <tr>
                  <td>大专&nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;2016-至今</td>
                </tr>
              </table>
              <!-- table3 -->
              <table class="t2">
                <tr>
                  <th>个人技能</th>
                </tr>
                <tr>
                  <td>Html</td>
                </tr>
                <tr>
                  <td>CSS </td>
                </tr>
                <tr>
                  <td>JavaScript</td>
                </tr>
                <tr>
                  <td>jQuery</td>
                </tr>
                <tr>
                  <td>Vue</td>
                </tr>
              </table>
              <!-- table4 -->
              <table class="t2">
                <tr>
                  <th>个人工作经历</th>
                </tr>
                <tr>
                  <td>16年在台山嘉明酒店做服务员(假期工)</td>
                </tr>
                <tr>
                  <td>17年在功夫客(台山四九店)做收银员(假期工)</td>
                </tr>
                <tr>
                  <td>18年在肇庆市睿客信息科技有限公司做实习生(学习前端)</td>
                </tr>
              </table>
            </div>
            <!-- 简历右边 -->
            <div class="p-c-right">
              <!-- card1 -->
              <el-row :gutter="12">
                <el-col :span="8">
                  <el-card shadow="hover" class="Recard">
                      <h2>求职意向</h2>
                      <p>期望的职业：前端开发工程师</p>
                      <p>掌握的技术：Html、JS等等 </p>
                  </el-card>
                </el-col>
              </el-row>
              <!-- card2 -->
              <el-row :gutter="12">
                <el-col :span="8">
                  <el-card shadow="always" class="Recard">
                      <h2>兴趣爱好</h2>
                      <p>做网站、唱歌、打羽毛球、玩游戏</p>
                      <p>关注娱乐新闻</p>
                  </el-card>
                </el-col>
              </el-row>
              <!-- card3 -->
              <el-row :gutter="12">
                <el-col :span="8">
                  <el-card shadow="hover" class="Recard">
                      <h2>校园经历</h2>
                      <p>参加羽毛球社团</p>
                      <p>参加2018穿越火线百城联赛，团队止步于省赛 </p>
                      <p>参加2018鼎湖校区的夜市活动，主要卖荧光棉花糖、小吃 </p>
                  </el-card>
                </el-col>
              </el-row>
              <!-- card4 -->
              <el-row :gutter="12">
                <el-col :span="8">
                  <el-card shadow="always" class="Recard">
                      <h2>自我评价</h2>
                      <p>喜欢IT行业，保持着一颗请教学习的心</p>
                      <p>责任心强，社交能力较好</p>
                  </el-card>
                </el-col>
              </el-row>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LeaderComponent from "../leader";
export default {
  name: "rehead",
  data() {
    return {
      show2: true
    };
  },
  created() {},
  components: {
    LeaderComponent
  }
};
</script>



<style scoped>
.leader {
  background: url("./img/ReheadBG.jpg");
  overflow: hidden;
  color: white;
}

.content {
  width: 100%;
  height: 100%;
  background-color: #f3f3f3;
  overflow: hidden;
}
.paper {
  width: 210mm;
  /* height: 100%; */
  height: 260mm;
  margin: 30px auto;
  background-color: white;
  box-shadow: 0px 0px 15px #888888;
  overflow: hidden;
}
.box {
  width: 95%;
  height: 90%;
  margin: auto;
}
.box h1 {
  margin-top: 20px;
  margin-bottom: 10px;
  font-weight: 600;
  font-size: 2rem;
}
.p-head {
  display: flex;
  justify-content: space-between;
  color: #8b8b8b;
  font-weight: 550;
}
.orange {
  color: #f89f63;
  font-weight: 550;
  padding-right: 5px;
  font-size: 14px;
}

.p-h-left span {
  color: #f89f63;
  font-weight: 550;
  padding-right: 5px;
}

.p-h-center {
  width: 50%;
}
.p-h-center p {
  font-size: 12px;
  /* margin: 0px 35px; */
}

.p-h-photo {
  height: 70px;
}
.p-h-photo img {
  position: relative;
  width: 130px;
  height: 130px;
  border-radius: 50%;
  top: -50px;
}

.p-content {
  display: flex;
}
/*表格*/
td {
  width: 220px;
  border-bottom: 1px solid #b1b1b1;
  text-align: left;
  padding-top: 10px;
  color: #6b6b6b;
  font-size: 14px;
}
th {
  width: 220px;
  border-bottom: 1px solid #b1b1b1;
  text-align: left;
  padding-top: 10px;
  color: #6b6b6b;
  font-size: 17px;
}
.t2 {
  margin: 20px 0;
}

.transition-box {
  margin-bottom: 10px;
  width: 200px;
  height: 100px;
  border-radius: 4px;
  background-color: #409eff;
  text-align: center;
  color: #fff;
  padding: 40px 20px;
  box-sizing: border-box;
  margin-right: 20px;
}
.Recard{
    width: 450px;
    margin: 30px 0 0 30px;
    text-align: center;
}
.Recard h2{
    
    font-size: 20px;
    padding-bottom: 5px;
}
.Recard p{
  padding-bottom: 5px;
}
</style>
