<template>
  <div class="home">
    <div id="eyecatch">
      <Header></Header>
      <div class="title">
        <h1>FUKAGAWA-TEI</h1>
        <p>下町・深川の美味しいがそこにある</p>
      </div>
      <div class="number-box">
        <img class="logo" src="../assets/IMG_0674.gif">
        <div>
          <p>ご予約の方はこちらの電話番号まで</p>
          <a href="tel:080-1111-2222" id="number">080-1111-2222</a>
        </div>
      </div>
    </div>
    <div class="flex">
      <h1 class="big-title">CONCEPT</h1>
      <div class="concept-box">
        <div class="concept-content">
          <h1>下町の小さなレストラン・深川亭</h1>
          <p>2002年の創業以来、シェフのこだわりは</p>
          <ol>
            <li>無農薬や低農薬の野菜</li>
            <li>天然物の魚介類で安心</li>
            <li>安全の素材を使った調理</li>
          </ol>
        </div>
        <div class="concept-img">
          <img src="../assets/bamboo-828703_1920.jpg">
          <img src="../assets/bridge-53769_1920.jpg">
        </div>
      </div>
    </div>
    <div class="flex">
      <h1 class="big-title">MENU</h1>
      <div class="menu-card">
        <img src="../assets/bamboo-828703_1920.jpg">
        <div class="menu-content">
          <h1>・ジュージュー焼き</h1>
          <p>玉ねぎ、長ネギ、豚肉を煮込み、</p>
          <p>熱々の南部鉄器に乗せ、</p>
          <p>溶き卵をかけた料理です。</p>
        </div>
      </div>
      <div class="menu-card">
        <div class="menu-content">
          <h1>・深川丼</h1>
          <p>深川丼はアオヤギを使った</p>
          <p>当店自慢の下町・深川の伝統食</p>
          <p>文献に残る明治初期の</p>
          <p>深川丼を再現しました。</p>
        </div>
        <img src="../assets/bamboo-828703_1920.jpg">
      </div>
    </div>
  </div>
</template>

<script>
import Header from '../components/Header'
export default {
  components: {
    Header,
  }
}
</script>

<style scoped>
.home{
  background: url("../assets/fancy_deboss_@2X.png");
  /* Background pattern from Toptal Subtle Patterns */
}

/* アイキャッチ */

#eyecatch{
  width: 100%;
  height: 100vh;
  background-image: url("../assets/tori-1976609_1920.jpg");
  background-size: cover;
  position: relative;
}
.title{
  text-align: center;
}
.title h1{
  margin-top: 70px;
  font-size: 50px;
}
.title p{
  font-size: 30px;
}
.number-box{
position: absolute;
bottom: 0;
right: 0;
display: flex;
align-items: center;
height: 110px;
width: 300px;
padding: 20px;
background: rgb(253, 253, 253);
}
.number-box p{
  margin-left: 20px;
  font-size: 20px;
  color: black;
}
#number{
  margin: 20px 30px 0;
  color: black;
  font-size: 17px;
}

/* コンセプト */

.big-title{
  font-size: 40px;
  opacity: 0.7;
  margin: 200px 0 50px;
}
.concept-box{
  display: flex;
  justify-content: center;
  align-items: center;
}
.concept-content{
  width: 60%;
  padding: 0 70px;
}
.concept-content h1{
  font-size: 25px;
  margin-bottom: 50px;
}
.concept-content p{
  font-size: 20px;
  line-height: 1.7;
}
.concept-content ol {
  color: #472b00;
  border-top: solid #472b00 1px;/*上のボーダー*/
  border-bottom: solid #472b00 1px;/*下のボーダー*/
  padding: 0.5em 0 0.5em 1.5em;
}

.concept-content ol li {
  line-height: 1.5;
  padding: 0.5em 0;
  font-size: 25px;
}
.concept-img{
  width: 40%;
}

/* メニュー */

.menu-card{
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 100px;
}
.menu-card img{
  width: 50%;
}
.menu-content{
  width: 30%;
  margin-left: 5%;
}
.menu-content h1{
  font-size: 30px;
  margin-bottom: 30px;
}
.menu-content p{
  line-height: 2;
}
</style>
