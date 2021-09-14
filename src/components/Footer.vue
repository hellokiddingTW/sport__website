<template>
  <div class="footer">
    <ul class="footer__lists">
      <li
        class="footer__list"
        @click="footerClicked = 'home'"
        :class="{ clicked: footerClicked == 'home' }"
      >
        <span class="material-icons"> home </span>
        <p>大廳</p>
      </li>
      <li
        class="footer__list"
        @click="footerClicked = 'live_tv'"
        :class="{ clicked: footerClicked == 'live_tv' }"
      >
        <span class="material-icons"> live_tv </span>
        <p>主播賽事</p>
      </li>
      <li
        class="footer__list"
        @click="footerClicked = 'emoji_events'"
        :class="{ clicked: footerClicked == 'emoji_events' }"
      >
        <span class="material-icons"> emoji_events </span>
        <p>排行</p>
      </li>
      <li
        class="footer__list"
        @click="footerClicked = 'assignment'"
        :class="{ clicked: footerClicked == 'assignment' }"
      >
        <span class="material-icons"> assignment </span>
        <p>投注記錄</p>
      </li>
      <li class="footer__list"
      @click="footerClicked = 'face'"
        :class="{ clicked: footerClicked == 'face' }">
        <span class="material-icons"> face </span>
        <p>個人資料</p>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      footerClicked: "",
    };
  },
};
</script>

<style lang="scss" scoped>
.footer {
  background-color: #3c3c3c;
}
.footer__lists {
  display: flex;
  justify-content: space-around;
  .footer__list {
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-direction: column;
    padding: 1rem 0.5rem;
    cursor: pointer;
    span {
      color: #7b7b7b;
      text-align: center;
      margin-bottom: 0.25rem;
    }
    p {
      color: #7b7b7b;
      font-size: 12px;
      margin-bottom: 0;
    }
  }
  .clicked {
    span,
    p {
      color: #ffffff;
    }
  }
}
</style>