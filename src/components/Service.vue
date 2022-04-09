<template>
  <div>
    <section id="service">
      <h2>{{ service.title }}</h2>
      <div class="imageText">
        <div class="image"><img :src="service.image1" alt="" srcset="" /></div>
        <div class="text">
          <h3 v-html="service.subTitle1"></h3>
          <p v-html="service.description1"></p>
        </div>
      </div>
      <div class="imageText">
        <div class="text">
          <h3 v-html="service.subTitle2"></h3>
          <p v-html="service.description2"></p>
        </div>
        <div class="image"><img :src="service.image2" alt="" srcset="" /></div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "AbeService",
  data: () => {
    return {
      service: {
        title: "Service",
        subTitle1: "リリース時のサポートで<br>サービスのブランディングを",
        subTitle2: "リリース後のサポートで<br>効果を最大化させる",
        image1: require(`@/assets/images/task/1DE22718-1670-4CFB-90DC-E8B14F0DE10C_1_105_c.jpeg`),
        image2: require(`@/assets/images/task/FFA55F6A-A7EB-4B82-9712-475F4784E8A3_1_105_c.jpeg`),
        description1:
          "弊社では、リリース時もサポートさせて頂きます。プレスリリース用のサイトや動画制作を通して、サービスのブランディングを行わせて頂きます。",
        description2:
          "弊社では、リリース後もサポートさせて頂きます。サービスはリリース後に様々な課題にぶつかります。そこでクライアント様と一緒に改善を行うことで、デザインの効果を最大化させます。",
      },
    };
  },
};
</script>

<style scoped>
h2 {
  text-align: center;
  letter-spacing: 6px;
  line-height: 2;
  font-family: "Roboto", sans-serif;
  font-size: 36px;
  letter-spacing: 1.4px;
  margin-bottom: 70px;
  margin-top: 0;
}
#service {
  margin-left: 200px;
  margin-right: 200px;
}
#service .imageText {
  display: flex;
  justify-content: space-between;
}
.image {
  flex: none;
  overflow: hidden;
  transition: 0.3s;
}
#servisce .image img {
  height: 450px;
  width: 340px;
  transition: 0.3s;
}
.image img:hover {
  transform: scale(1.3);
}
.text {
  margin-left: 180px;
  margin-top: 80px;
  padding: 0 !important;
}
h3 {
  margin-bottom: 45px;
}
.image img {
  height: 450px;
  width: 340px;
  transition: 0.3s;
}
.text {
  padding: 0 !important;
}
.imageText + .imageText {
  margin-top: 50px;
}

@media screen and (max-width: 959px) {
  .text {
    flex-direction: column;
  }
  text {
    padding: 0 !important;
  }
}
</style>
