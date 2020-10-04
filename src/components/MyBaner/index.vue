<template>
  <div>
    <div class="firstDiv">
      <div>
        <img :src="firstImg" class="first" />
      </div>
      <div class="span">Рекламная сеть</div>
    </div>
    <div>
      <img :src="secondImg" class="second" />
    </div>
    <div class="spanSec">Соковита хурма</div>
  </div>
</template>

<script>
export default {
  name: "MyBanner",
  props: {
    firstImg: {
      type: String,
      default:
        "https://ppobzor.ru/wp-content/uploads/2018/06/recreativ-logo.jpg",
    },
    secondImg: {
      type: String,
      default:
        "https://smak.ua/i/51/82/7/51827/gallery/b212d499e270fa5678442087e7238926-quality_100Xresize_1Xallow_enlarge_0Xw_700Xh_0.jpg",
    },
  },
};
</script>

<style lang="css" scoped>
div {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.first {
  width: 200px;
}
.firstDiv {
  color: aliceblue;
  font-size: 30px;
  font-style: italic;
  display: flex;
  background-color: #2c3e50;
  width: 700px;
  justify-content: space-between;
  flex-direction: row;
}
.span {
  padding-right: 30px;
}
.spanSec {
  color: aqua;
  font-size: 30px;
}
</style>