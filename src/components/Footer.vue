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

<style>
@media screen and (max-width: 500px) {
  .footer {
    background-color: black;
    color: #fff;
    width: 100%;
    height: 60px;
  }
  .footer p {
    padding-top: 18px;
  }
}

@media screen and (min-width: 501px) {
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
}
</style>
