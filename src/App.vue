<template>
  <div id="app">

  <header>
    <div class="container">
      <div class="header-left">
        <p>Travelmate</p>
      </div>
      <div class="header-right">
        <a href="#" class="login">ログイン</a>
      </div>
    </div>
  </header>

    <div class="top-wrapper">
      <div class="container">
        <div class="text1">
          <h1>{{message1}}</h1>
          <h1>{{message2}}</h1>
        </div>
        <br>
        <div class="btn-wrapper">
          <a href="#" class="btn signup">新規登録はこちら</a>
          <p>or sign up with</p>
          <a href="#" class="btn facebook"><span class="fa fa-facebook"></span>Facebookで登録</a>
          <a href="#" class="btn twitter"><span class="fa fa-twitter"></span>Twitterで登録</a>
        </div>
      </div>
    </div>

    <div class="about-wrapper">
      <div class="container">
        <br><br><br>
        <h1>{{about1}}</h1>
        <br>
        <h1>{{about2}}</h1>
        <br>
        <div class="frame">
        <img v-bind:src="fileName0" width=700px height=500px></img>
        </div>
        <br><br><br>
        <h2>{{about3}}</h2>
        <br>
        <h3>{{about4}}</h3>
        <h3>{{about5}}</h3>
        <h3>{{about6}}</h3>
      </div>
    </div>

    <div class="lesson-wrapper">
      <div class="container">
        <div class="heading">
          <h2>{{message4}}</h2>
        </div>
        <div class="lessons">
          <div class="lesson">
            <div class="lesson-icon">
              <img v-bind:src="fileName1"></img>
              <p>旅先に友達が！</p>
            </div>
            <p class="txt-contents">{{merit1}}</p>
          </div>
          <div class="lesson">
            <div class="lesson-icon">
              <img v-bind:src="fileName2"></img>
              <p>ディープな観光！</p>
            </div>
            <p class="txt-contents">{{merit2}}</p>
          </div><div class="lesson">
            <div class="lesson-icon">
              <img v-bind:src="fileName3"></img>
              <p>語学力向上！</p>
            </div>
            <p class="txt-contents">{{merit3}}</p>
          </div><div class="lesson">
            <div class="lesson-icon">
              <img v-bind:src="fileName4"></img>
              <p>完全無料！</p>
            </div>
            <p class="txt-contents">{{merit4}}</p>
          </div>
        </div>
      </div>
    </div>

    <div class="message-wrapper">
      <div class="container">
        <div class="heading">
        <h3>{{message5}}</h3>
        </div>
        <span class="btn message">さっそく旅仲間を探す</span>
      </div>
    </div>

    </div>
</template>

<script>
import ToDoItem from './components/ToDoItem.vue'
import Logo from './assets/logo.png';
export default {
  name: 'to-do',
  components: {
    ToDoItem
  },
  data() {
      return {
          message1:'Have a wonderful travel',
          message2:'with a wonderful travelmate!',
          message4:'Travelmateを利用する4つのメリット',
          message5:"Let's make travelmates all over the world!",
          about1:'Travelmateは旅行者と現地の人々をマッチングするサービス。',
          about2:'旅行先での出会いが、あなたの旅の思い出に。',
          about3:'Travelmateの使い方はとってもシンプル！',
          about4:'①Travelmateのアプリをインストール',
          about5:'②行きたい旅行先を指定',
          about6:'③マッチングしたトラベルメイト（旅行仲間）と現地で合流！',
          fileName0:'IMG_2327.jpg',
          fileName1:'https://prog-8.com/images/html/advanced/html.png',
          fileName2:'https://prog-8.com/images/html/advanced/jQuery.png',
          fileName3:'https://prog-8.com/images/html/advanced/ruby.png',
          fileName4:'https://prog-8.com/images/html/advanced/php.png',
          merit1:'「せっかくのひとり旅だし、現地の人とたくさん交流したい！」そう思っていても意外に店の定員さんは忙しそうだったり、そんな人当たりのいいあなたを狙う詐欺師がいたり...。Travelmateは安全に現地の人と関われる機会を提供します。',
          merit2:'日本語のガイドブックに載ってる観光地、ハズレはないけれどインスタでも見たような...。現地に住むトラベルメイトの案内は、あなたの旅を普通の日本人が経験できないような個性あふれるものにしてくれます。',
          merit3:'「せっかくの海外だし、学校で勉強している英語を頑張って話してみよう！」そう意気込んで現地についたら、ネイティヴの会話スピードに唖然ということも。Travelmateはあらかじめ言語レベルを知った状態でマッチできるので、より気楽に会話を楽しめます。',
          merit4:'Travelmateのサービスはポイント制で、自分が日本で外国人を案内することによって得られるポイントで自分が旅行した時の案内を受けることができます。コストをかけずにあなたの旅の楽しさを最大限に引き出すことができます。',
      }
  },
}
</script>

<style>
  body {
    margin: 0;
    font-family: "Hiragino Kaku Gothic ProN";
  }

  a {
    text-decoration: none;
  }

  .container {
    width: 1170px;
    padding: 0 15px;
    margin: 0 auto;
  }

  .top-wrapper {
    padding: 180px 0 100px 0;
    background-image: url('63993e9cf9d8d01ec81affe1281ebfa2_m.jpg');
    background-size: cover;
    color: white;
    text-align: center;
  }

  .top-wrapper h1 {
    opacity: 1;
    font-size: 70px;
    letter-spacing: 5px;
    font-family: 'cursive',Comic Sans MS;
  }

  .top-wrapper p {
    opacity: 1;
  }

  .btn-wrapper {
    margin: 20px 0;
  }

  .btn-wrapper p {
    margin: 10px 0;
  }

  .signup {
    background-color: #239b76;
  }

  .facebook {
    background-color: #3b5998;
    margin-right: 10px;
  }

  .twitter {
    background-color: #55acee;
  }

  .btn {
    padding: 8px 24px;
    color: white;
    display: inline-block;
    opacity: 0.8;
    border-radius: 4px;
  }

  .btn:hover {
    opacity: 1;
  }

  .fa {
    margin-right: 5px;
  }

  header {
    height: 65px;
    width: 100%;
    background-color: rgba(34, 49, 52, 0.9);
    /* positionプロパティをfixedに、topを0に指定してください */
    position:fixed;
    top:0;
    /* z-indexを10に指定してください */
    z-index:10;
  }

  .logo {
    width: 124px;
    margin-top: 20px;
  }

  .header-left {
    float: left;
    color: white;
    font-family: 'cursive',Comic Sans MS;
    font-size: 18px;
  }

  .header-right {
    float: right;
    background-color: rgba(255, 255, 255, 0.3);
    transition: all 0.5s;
  }

  .header-right:hover {
    background-color: rgba(255, 255, 255, 0.5);
  }

  .header-right a {
    line-height: 65px;
    padding: 0 25px;
    color: white;
    display: block;
  }

  .lesson-wrapper {
    height: 500px;
    padding-bottom: 80px;
    background-color: #f7f7f7;
    text-align: center;
  }

  .heading {
    padding-top: 60px;
    padding-bottom: 30px;
    color: #5f5d60;
  }

  .heading h2 {
    font-weight: normal;
  }

  .lesson {
    float: left;
    width: 25%;
  }

  .lesson-icon {
    position: relative;
  }

  .lesson-icon p {
    position: absolute;
    top: 90px;
    width: 100%;
    color: white;
  }

  .txt-contents {
    width: 80%;
    display: inline-block;
    margin-top: 20px;
    font-size: 12px;
    color: #b3aeb5;
  }

  .heading h3 {
    font-weight: normal;
  }

  .message-wrapper {
    border-bottom: 1px solid #eee;
    padding-bottom: 80px;
    text-align: center;
  }

  .message {
    padding: 15px 40px;
    background-color: #5dca88;
    cursor: pointer;
    box-shadow: 0 7px #1a7940;
  }

  .message:active {
    position: relative;
    top: 7px;
    box-shadow: none;
  }

  footer img {
    width: 125px;
  }

  footer p {
    color: #b3aeb5;
    font-size: 12px;
  }

  footer {
    padding-top: 30px;
  }

  .text1 {
    color: #fff;
    text-stroke: 1px #000;
    -webkit-text-stroke: 3px #000;
  }

  .about-wrapper {
    height: 1100px;
    padding-bottom: 80px;
    background-color: white;
    text-align: center;
  }

  .frame {
	display: inline-block;
	box-shadow: 0px 0px 20px -5px rgba(0, 0, 0, 0.8);
  }

</style>
