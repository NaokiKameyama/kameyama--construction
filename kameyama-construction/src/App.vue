<template>
  <div>
    <div class="back">
      <div class="title">
        亀山建設
        <div class="sub-title">安心できる住まいづくりのために</div>
      </div>
    </div>
    <div class="company-discription-container">
      <div class="company-discription-title">会社情報</div>
      <div class="table-container">
        <table>
          <tr>
            <th>会社名</th>
            <td>亀山建設</td>
          </tr>
          <tr>
            <th>創業</th>
            <td>1940年</td>
          </tr>
          <tr>
            <th>代表</th>
            <td>亀山一義</td>
          </tr>
          <tr>
            <th>従業員数</th>
            <td>3人</td>
          </tr>
          <tr>
            <th>電話番号</th>
            <td>0256-73-2580</td>
          </tr>
          <tr>
            <th>所在地</th>
            <td>〒953-0061<br>新潟県新潟市西蒲区馬堀4668-3</td>
          </tr>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld';

export default {
  name: "App",

  components: {
    // HelloWorld,
  },

  data: () => ({
    //
  })
};
</script>

<style scoped>
.back {
  height: 90vh;
  width: 100vw;
  margin: auto auto;
  background-color: #486d46; /* 背景色 */
  background-image: url("~@/assets/hayate.jpg"); /* 画像 */
  background-size: cover; /* 全画面 */
  background-attachment: fixed; /* 固定 */
  background-position: center center; /* 縦横中央 */

  display: flex;
  justify-content: center; /*左右中央揃え*/
  align-items: center; /*上下中央揃え*/
}

.back::after {
  height: 90vh;
  width: 100vw;
  content: "";
  background-color: rgba(73, 73, 73, 0.651);
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
}

.title {
  font-size: 100px;
  color: #fff;
  font-weight: bold;
  position: relative;
  z-index: 1;
  text-align: center;
  border-top: double;
  border-bottom: double;
  width: 40%;
}

.sub-title {
  font-size: 20px;
}

.company-discription-container {
}

.company-discription-title {
  border-bottom: double;
  width: 30%;
  text-align: center;
  color: #52c2d0;
  font-weight: bolder;
  font-size: 40px;
  margin-top: 30px;
  text-align: center;
  margin-left:auto;
  margin-right:auto;
}

.table-container{
  margin-top: 30px;
  width: 50%;
  margin-left:auto;
  margin-right:auto;
  margin-bottom: 30px;
}

table{
  width: 100%;
  border-collapse: collapse;
}

table tr{
  border-bottom: solid 2px white;
}

table tr:last-child{
  border-bottom: none;
}

table th{
  position: relative;
  text-align: left;
  width: 10%;
  background-color: #52c2d0;
  color: white;
  text-align: center;
  padding: 10px 0;
}

table th:after{
  display: block;
  content: "";
  width: 0px;
  height: 0px;
  position: absolute;
  top:calc(50% - 10px);
  right:-10px;
  border-left: 10px solid #52c2d0;
  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
}

table td{
  text-align: left;
  width: 30%;
  text-align: center;
  background-color: #eee;
  padding: 10px 0;
  font-weight: bolder;
}

/*以下、レスポンシブデザイン用CSS*/
@media screen and (max-width: 700px) {
  /*スマホ用のcssを記述*/
  .title {
    font-size: 13vw;
    color: #fff;
    font-weight: bold;
    position: relative;
    z-index: 1;
    text-align: center;
    border-top: double;
    border-bottom: double;
    width: 80%;
  }

  .sub-title {
    font-size: 5vw;
  }

  .company-discription-container {
}

.company-discription-title {
  border-bottom: double;
  width: 50%;
  text-align: center;
  color: #52c2d0;
  font-weight: bolder;
  font-size: 30px;
  margin-top: 30px;
  text-align: center;
  margin-left:auto;
  margin-right:auto;
}

.table-container{
  margin-top: 30px;
  width: 80%;
  margin-left:auto;
  margin-right:auto;
  margin-bottom: 30px;
}

table{
  width: 100%;
  border-collapse: collapse;
}

table tr{
  border-bottom: solid 2px white;
}

table tr:last-child{
  border-bottom: none;
}

table th{
  position: relative;
  text-align: left;
  width: 10%;
  background-color: #52c2d0;
  color: white;
  text-align: center;
  padding: 10px 0;
}

table th:after{
  display: block;
  content: "";
  width: 0px;
  height: 0px;
  position: absolute;
  top:calc(50% - 10px);
  right:-10px;
  border-left: 10px solid #52c2d0;
  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
}

table td{
  text-align: left;
  width: 30%;
  text-align: center;
  background-color: #eee;
  padding: 10px 0;
  font-weight: bolder;
}
}

@media only screen and (min-width: 700px) and (max-width: 1023px) {
  /*tablet用のcssを記述*/
}
</style>
