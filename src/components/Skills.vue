<template>
  <div class="content" id="news">
    <h2 class="news">Skills</h2>
    <ul id="newNews">
      <li v-for="item in arrayNews" :key="item.message">
        <div class="image-x">
          <img
            src="@/assets/images/task/F3550BB1-9190-436E-B56C-97881339CD07_1_105_cのコピー.jpg"
            alt=""
            srcset=""
          />
        </div>
        <div class="text-x">
          <p>{{ item.message }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AbeSkills",
  data: function () {
    return {
      arrayNews: [
        { message: "news111" },
        { message: "news222" },
        { message: "news333" },
      ],
    };
  },
};
</script>

<style scoped>
@media screen and (max-width: 500px) {
  .content {
    text-align: initial;
    letter-spacing: 1.3px;
    margin-bottom: 150px;
  }
  h2 {
    text-align: center;
    letter-spacing: 2px;
  }
  .content p {
    text-align: initial;
    font-size: 14px;
    font-family: Noto Sans CJK JP;
    line-height: 2;
    letter-spacing: 1.2px;
    font-weight: bold;
  }
  #news {
    width: 100%;
    text-align: initial;
    letter-spacing: 1.3px;
    margin-bottom: 150px;
  }
  ul {
    list-style: none;
    padding-left: 0px;
  }
  .news {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    font-size: 36px;
    letter-spacing: 2px;
    font-weight: 600;
    margin-bottom: 70px;
  }
  #news ul li {
    display: list-item;
    box-shadow: 0px 0px 6px 1px rgba(0, 0, 0, 0.24);
    margin: 0 13px;
    width: 242px;
    height: auto;
    text-align: -webkit-match-parent;
  }
  .image-x {
    position: relative;
    margin: 0 0.5px;
    transition: 0.3s;
    overflow: hidden;
    width: 320px;
    height: 200px;
    transition-duration: 0.5s;
  }
  .image-x img {
    transition-duration: 0.5s;
  }
  .image-x:hover img {
    transform: scale(1.3);
    transition-duration: 0.5s;
    transition: 0.3s;
  }
  .text-x p {
    text-align: initial;
    font-size: 13.2px;
    font-family: Noto Sans CJK JP;
    line-height: 2;
    letter-spacing: 1.2px;
    font-weight: bold;
    padding-left: 25px;
    padding-right: 25px;
    padding-bottom: 20px;
    margin-bottom: 50px;
  }
}
@media screen and (min-width: 501px) {
  h2 {
    font-family: "Roboto", sans-serif;
    font-size: 36px;
    letter-spacing: 1.4px;
  }
  .content h2 {
    text-align: center;
    color: #000000;
    margin-bottom: 70px;
    margin-top: 0%;
  }
  .content p {
    font-size: 14px;
    letter-spacing: 1px;
    line-height: 30px;
    margin-top: 0px;
  }
  #news ul {
    list-style: none;
    justify-content: center;
  }
  #news {
    margin-top: 150px;
  }
  .news {
    margin-bottom: 100px;
  }

  #news ul li {
    box-shadow: 0px 0px 6px 1px rgba(0, 0, 0, 0.24);
    margin: 0 15px;
    display: inline-block;
  }

  .image-x {
    position: relative;
    margin: 0 0.5px;
    transition: 0.3s;
    overflow: hidden;
    height: 200px;
    transition-duration: 0.5s;
  }
  .image-x img {
    transition-duration: 0.5s;
  }
  .image-x:hover img {
    transform: scale(1.3);
    transition-duration: 0.5s;
    transition: 0.3s;
  }
  .text-x {
    width: 100%;
    height: 145px;
    padding: 25px 40px;
    box-sizing: border-box;
  }

  .text p {
    font-size: 13px;
    color: #000000;
    margin-right: 65px;
  }
}
</style>
