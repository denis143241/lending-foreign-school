<template>
  <div class="card">
    <div class="quote_and_line">
      <div class="quote"></div>
      <div class="line right line-bottom"></div>
    </div>
    <div class="content">
      <div class="title">{{ quote.name }}</div>
      <p :style="{ fontSize: `${size}px` }">{{ quote.quote }}</p>
    </div>
    <div class="quote_and_line">
      <div class="line left line-bottom"></div>
      <div class="quote left"></div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    quote: {
      type: Object,
    },
  },
  computed: {
    size() {
      return this.quote.quote.length > 150 ? 20 : 22;
    },
  },
};
</script>

<style lang="less" scoped>
@import url("../assets/mainStyle.less");
.card {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 300px;
  max-height: 300px;
  background-color: #f1968f;
  padding: 10px;
  color: #000;
}
.content {
  flex-grow: 2;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.title {
  text-align: center;
  font-family: @main-font;
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 20px;
}
p {
  text-align: center;
  font-family: @dop-font;
  font-size: 22px;
  font-weight: 300;
}
.quote {
  background: url("../assets/quotes.png") no-repeat center center;
  background-size: 100%;
  width: 40px;
  height: 40px;
  display: inline-block;
}
.quote_and_line {
  position: relative;
  height: 40px;
}
.line {
  height: 3px;
  width: 86%;
  background-color: #000;
  display: inline-block;
  &-bottom {
    margin-top: 18px;
    margin-right: 4%;
  }
  &-top {
    margin-bottom: 17px;
    margin-left: 4%;
  }
}

@media only screen and (max-width: 600px) {
  .card {
    height: 100%;
    max-height: 100%;
  }
  p {
    font-size: 16px !important;
  }
  .quote_and_line {
    display: flex;
  }
}
</style>
