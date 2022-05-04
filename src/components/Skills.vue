<template>
  <div class="content" id="news">
    <h2 class="news">Skills</h2>
    <h3>Languages/flameworks</h3>
    <ul id="newNews">
      <li v-for="item in arraySkills" :key="item.message">
        <div class="skills">
          <div class="text-x">
            <span>{{ item.message }}</span>
            <div class="skill">
              <v-progress-linear v-model="item.value" rounded>{{
                item[0]
              }}</v-progress-linear>
              <div class="text-number">{{ item.value }}%</div>
            </div>
          </div>
        </div>
      </li>
    </ul>

    <h3>Others</h3>
    <ul>
      <li v-for="item in arrayOthers" :key="item.message">
        <div class="skill">
          <div class="text-x">
            <span>{{ item.message }}</span>
            <div>
              <v-progress-linear v-model="item.value" rounded
                >{{ item[0] }}
                <p>{{ item.value }}%</p></v-progress-linear
              >
            </div>
          </div>
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
      arraySkills: [
        { message: "HTML/CSS", value: 50 },
        { message: "Java Script", value: 50 },
        { message: "PHP", value: 30 },
        { message: "Vue.js", value: 50 },
        { message: "React.js", value: 40 },
      ],
      arrayOthers: [{ message: "GitHub", value: 60 }],
    };
  },
};
</script>

<style lang="scss" scoped>
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
    width: 300px;
    height: auto;
    text-align: -webkit-match-parent;
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
    margin-bottom: 40px;
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
    padding: 0;
    margin-bottom: 60px;
  }
  #news {
    margin-top: 150px;
    text-align: center;
  }
  .news {
    margin-bottom: 100px;
  }
  h3 {
    margin-bottom: 40px;
    letter-spacing: 1px;
  }
  #news ul li {
    box-shadow: 0px 0px 6px 1px rgba(0, 0, 0, 0.24);
    margin: 0 15px;
    display: inline-block;
  }
  .text-x {
    width: 350px;
    height: 80px;
    padding: 15px;
    box-sizing: border-box;
  }

  .text p {
    font-size: 13px;
    color: #000000;
    margin-right: 65px;
  }
  .skill {
    color: #606266;
    display: flex;
    vertical-align: middle;
    line-height: 1;
    padding: 3px;
  }
}
</style>
