<template>
  <div class="header">
    <div class="inner">
      <div class="logo">
        <p>Ryohei Abe</p>
      </div>
      <ul class="menu">
        <li><a href="#about">About</a></li>
        <li><a href="#news">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AbeHeader",
};
</script>

<style scoped>
.header {
  background: #000000;
  border-bottom: solid 1px #ffffff;
}
.inner {
  display: flex;
  align-items: center;
  margin: auto;
  max-width: 1200px;
}
/* @media screen and (max-width: 500px) {
  flex-direction:column;
} */

.logo p {
  color: #fff;
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 0%;
}
ul.menu {
  display: flex;
  margin-left: auto;
  list-style: none;
}
/* @media screen and (max-width: 500px) {
  margin-left: unset;
} */

li {
  padding: 12px;
}
a {
  color: #ffffff;
  font-size: 18px;
  font-weight: bold;
}
</style>
