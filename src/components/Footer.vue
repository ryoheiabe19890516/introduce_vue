<template>
  <div class="footer">
    <p>©︎Ryohei Abe all rights reserved</p>
  </div>
</template>

<script>
export default {
  name: "AbeFooter",
};
</script>

<style lang="scss" scoped>
@media screen and (max-width: 500px) {
  .footer {
    background-color: black;
    width: 100%;
    height: 60px;
    p {
      padding-top: 18px;
      text-align: center;
      color: #fff;
    }
  }
}
@media screen and (min-width: 501px) {
  .footer {
    width: 100%;
    background-color: #1b1310;
    p {
      color: #fff;
      font-size: 14px;
      text-align: center;
      margin-top: 25px;
    }
  }
}
</style>
