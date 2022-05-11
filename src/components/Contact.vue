<template>
  <v-app>
    <div>
      <section class="content" id="contact">
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
  </v-app>
</template>

<script>
export default {
  name: "AbeContact",
  data: function () {
    return {
      Moldon: "あべ阿部アベ",
    };
  },
};
</script>

<style lang="scss" scoped>
h2 {
  font-family: "Roboto", sans-serif;
  font-size: 36px;
  letter-spacing: 1.4px;
}
.content h2 {
  text-align: center;
  color: #000000;
  margin-bottom: 40px;
  margin-top: 0%;
}
@media screen and (min-width: 501px) {
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
    .button:hover {
      box-shadow: none;
      color: #000000;
      background: #ffffff;
    }
  }
  form {
    text-align: center;
    border-width: thick;
  }

  input {
    resize: none;
    width: 700px;
    border-style: groove;
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
