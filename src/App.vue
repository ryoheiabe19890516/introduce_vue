<template>
  <v-app>
    <div class="task" id="abeTaskSp">
      <AbeHeader />
      <div class="mainVisual">
        <h1>Portfolio<br />of<br />Ryohei ABE</h1>
      </div>
      <div class="content-wrapper">
        <section class="content" id="about">
          <h2 id="target" class="targetClass">{{ about.title }}</h2>
          <h3>{{ about.description }}<br />{{ about.more }}</h3>
          <p>{{ about.detail }}</p>
        </section>

        <!-- <section class="content" id="service">
        <AbeService />
      </section> -->

        <section class="content" id="news"><Skills /></section>

        <section id="contact">
          <h2>お問い合わせ</h2>
          <form action="">
            <div class="input4">
              <div>
                <dl class="input">
                  <dt>{{ Moldon }}</dt>
                  <dd><input type="text" style="" value="" /></dd>
                </dl>
              </div>
              <div>
                <dl class="input">
                  <dt>電話番号</dt>
                  <dd><input type="text" style="" value="" /></dd>
                </dl>
              </div>
              <div>
                <dl class="input">
                  <dt>メールアドレス</dt>
                  <dd><input type="text" style="" value="" /></dd>
                </dl>
              </div>
              <div>
                <dl class="textarea">
                  <dt>お問い合わせ内容</dt>
                  <dd class="area">
                    <input type="textarea" style="height: 171px" value="" />
                  </dd>
                </dl>
              </div>
            </div>
          </form>
          <input type="submit" value="送信" class="button" />
        </section>
      </div>
    </div>
    <v-main> </v-main>
    <AbeFooter />
  </v-app>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";
// import Service from "./components/Service.vue";
import AbeHeader from "./components/AbeHeader.vue";
import Skills from "./components/Skills.vue";
import AbeFooter from "./components/Footer.vue";

export default {
  name: "App",

  components: {
    // HelloWorld,
    // Service,
    AbeHeader,
    Skills,
    AbeFooter,
  },

  data: function () {
    return {
      about: {
        title: "About me",
        description: "ミニマルで",
        more: "洗練されたデザインを。",
        detail:
          "近年、ミニマルなデザインが流行しています。そこで弊社では、クライアント企業様新規サービス等の課題に対してミニマルで洗練されたデザインを実現させることで解決のサポートを致します。もちろん全てのサービスにおいてミニマルなデザインが課題解決になるわけではないので、課題や今後のサービスの展開等しっかりとヒアリングを行なった上でご提案させて頂きます。",
      },
      service: {
        title: "Service",
        description: "リリース時のサポートで",
        more: "サービスのブランディングを",
        detail:
          "弊社では、リリース後もサポートさせていただきます。プレスリリース用のサイトや動画制作を通して、サービスのブランディングを行わせて頂きます。",
        imgSrc: require("@/assets/images/task/1DE22718-1670-4CFB-90DC-E8B14F0DE10C_1_105_c.jpeg"),
      },
      imageTaxt: {
        description: "リリース後のサポートで",
        more: "効果を最大化させる",
        detail:
          " 弊社では、リリース後もサポートさせていただきます。サービスはリリース後に様々な課題にぶつかります。そこでクライアント様と一緒に改善を行うことで、デザインの効果を最大化させます。",
        imgSrc: require("@/assets/images/task/FFA55F6A-A7EB-4B82-9712-475F4784E8A3_1_105_c.jpeg"),
      },
      Moldon: "あべ阿部アベ",
    };
  },
};
</script>

<style lang="scss" scoped>
@media screen and (max-width: 500px) {
  .mainVisual {
    max-width: 100%;
    height: 768px;
    background-image: url("~@/assets/images/task/09EA34C6-F3C9-4FC7-9F6C-9E8759588E05_1_105_c111.jpeg");
    background-repeat: no-repeat;
    position: relative;
    margin-bottom: 100px;
    margin-top: 1px;
  }
  .mainVisual h1 {
    text-align: center;
    width: 300px;
    height: 125px;
    color: #fff;
    font-size: 30px;
    border: 2px solid #fff;
    position: absolute;
    top: 46%;
    left: 87px;
  }
  .content {
    text-align: initial;
    letter-spacing: 1.3px;
    margin-bottom: 150px;
  }
  h2 {
    text-align: center;
    letter-spacing: 2px;
  }
  #target {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    font-size: 36px;

    font-weight: 600;
    margin-bottom: 75px;
  }

  h3 {
    text-align: center;
    letter-spacing: 6px;
    line-height: 2;
  }
  .content p {
    text-align: initial;
    font-size: 14px;
    font-family: Noto Sans CJK JP;
    line-height: 2;
    letter-spacing: 1.2px;
    font-weight: bold;
  }
  #service .imageText .image-y {
    flex: none;
    overflow: hidden;
    width: 345;
    height: 150px;
  }
  #service .imageText .image-y img {
    transition: 0.3s;
    width: 100%;
    display: flex;
    flex-direction: column-reverse;
  }
  #service .imageText .image-y img:hover {
    transform: scale(1.3);
  }
  .icon {
    color: #fff;
    font-size: 26px;
    padding-top: 20px;
    padding-bottom: 18px;
    padding-right: 215px;
  }
  .service {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    font-size: 36px;
    letter-spacing: 2px;
    font-weight: 600;
    margin-bottom: 75px;
  }
  .image img {
    width: 345px;
    height: 150px;
  }
  #service .imageText .image {
    flex: none;
    overflow: hidden;
    width: 345;
    height: 150px;
  }
  #service .imageText .image img {
    transition: 0.3s;
    width: 345px;
  }
  #service .imageText .image img:hover {
    transform: scale(1.3);
  }
  .textMoldon {
    text-align: justify;
  }
  .image-y img {
    width: 100%;
    height: 150px;
  }

  .input4 {
    margin-top: 75px;
    margin-right: 35px;
  }
  input {
    width: 345px;
    height: 30px;
    padding-right: 10px;
  }

  .dt {
    font-size: 16px;
    padding-right: 170px;
  }
  .button {
    width: 235px;
    height: 59px;
    display: block;
    margin: 0 auto;
    border-radius: 40px;
    font-size: 15pt;
    font-weight: bold;
    text-align: center;
    padding: 16px 47px;
    margin-top: 50px;
    margin-bottom: 45px;
    background: #000000;
    color: #ffffff;
    line-height: 7px;
    transition: 0.3s;
    box-shadow: 0px 0px 6px 1px rgba(0, 0, 0, 0.24);
    border: 2px solid #000000;
    height: 60px;
  }
  .button:hover {
    box-shadow: none;
    color: #000000;
    background: #ffffff;
  }
}

/* 以下 min-width 500  */

@media screen and (min-width: 501px) {
  h1,
  h3,
  p {
    font-family: "Noto toians JP", sans-serif;
    letter-spacing: 1px;
  }

  h2 {
    font-family: "Roboto", sans-serif;
    font-size: 36px;
    letter-spacing: 1.4px;
  }

  h3 {
    font-weight: 400;
    line-height: 2;
  }

  /* header */

  .mainVisual {
    max-width: 100%;
    height: 1067px;
    background: url("~@/assets/images/task/09EA34C6-F3C9-4FC7-9F6C-9E8759588E05_1_105_c.jpeg");
    background-size: cover;
    position: relative;
    margin-bottom: 100px;
  }
  .mainVisual h1 {
    text-align: center;
    width: 445px;
    height: 205px;
    color: #fff;
    font-size: 45px;
    border: 2px solid #fff;
    position: absolute;
    top: 48%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%); /* Safari用 */
    transform: translate(-50%, -50%);
  }
  .mainVisual:active {
    background-image: url(https://wp-p.info/reps/css-intermediate/img/04_02.jpg);
  }
  p span {
    color: white;
  }
  p:hover span {
    color: red;
  }
  #service {
    margin-top: 150px;
  }
  #service .imageText .image-y {
    flex: none;
    overflow: hidden;
    width: 345px;
    height: 150px;
  }
  #service .imageText .image-y img {
    transition: 0.3s;
    width: 345px;
  }
  #service .imageText .image-y img:hover {
    transform: scale(1.3);
  }
  .service {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    font-size: 36px;
    letter-spacing: 2px;
    font-weight: 600;
    margin-bottom: 75px;
  }
  .imageText {
    flex-direction: column-reverse;
    display: flex;
  }
  .image img {
    width: 100%;
    height: 150px;
  }
  .text h3 {
    margin-top: 55px;
  }
  .text p {
    margin-top: 34px;
    margin-bottom: 40px;
  }

  #service .imageText .image {
    flex: none;
    overflow: hidden;
    width: 345px;
    height: 150px;
    flex-direction: column-reverse;
  }
  #service .imageText .image img {
    transition: 0.3s;
    width: 100%;
  }
  #service .imageText .image img:hover {
    transform: scale(1.3);
  }
  .content h2 {
    text-align: center;
    color: #000000;
    margin-bottom: 70px;
    margin-top: 0%;
  }
  .content h3 {
    font-size: 24px;
    margin-top: 10px;
    padding-left: 0px;
    padding-right: 0px;
    /* padding-bottom: 5px; */
    letter-spacing: 3px;
  }

  .content p {
    font-size: 14px;
    letter-spacing: 1px;
    line-height: 30px;
    margin-top: 0px;
  }
  #about {
    margin-left: 200px;
    margin-right: 200px;
  }
  h4 {
    text-align: center;
    font: size 500px;
  }

  .footer {
    width: 100%;
    height: 74px;
    background-color: #1b1310;
    border-bottom: 2px solid #fff;
  }
  .footer p {
    color: #fff;
    font-size: 14px;
    text-align: center;
    margin-top: 29px;
    padding: 29px;
    padding-bottom: 31px;
  }

  form {
    text-align: center;
    border-width: thick;
  }

  input {
    resize: none;
    width: 700px;
  }

  dt {
    text-align: left;
    padding-left: 380px;
  }
  .button {
    width: 235px;
    height: 59px;
    display: block;
    margin: 0 auto;
    border-radius: 40px;
    font-size: 15pt;
    font-weight: bold;
    text-align: center;
    padding: 16px 47px;
    margin-top: 50px;
    margin-bottom: 45px;
    background: #000000;
    color: #ffffff;
    line-height: 7px;
    transition: 0.3s;
    box-shadow: 0px 0px 6px 1px rgba(0, 0, 0, 0.24);
    border: 2px solid #000000;
    height: 60px;
  }
  .button:hover {
    box-shadow: none;
    color: #000000;
    background: #ffffff;
  }
}
</style>
