<template>
  <div class="videobar container">
    <h2 class="vb__title">在線主播</h2>
    <ul class="videobar__videos">
      <li class="vb__video">
        <a href="#">
          <img src="https://randomuser.me/api/portraits/women/72.jpg" alt="" />
          <p>Erica</p>
        </a>
      </li>
      <li class="vb__video">
        <a href="">
          <img src="https://randomuser.me/api/portraits/women/70.jpg" alt="" />
          <p>Erica</p>
        </a>
      </li>
      <li class="vb__video">
        <a href="">
          <img src="https://randomuser.me/api/portraits/women/17.jpg" alt="" />
          <p>Erica</p>
        </a>
      </li>
      <li class="vb__video">
        <a href="">
          <img src="https://randomuser.me/api/portraits/women/71.jpg" alt="" />
          <p>Erica</p>
        </a>
      </li>
      <li class="vb__video">
        <a href="">
          <img src="https://randomuser.me/api/portraits/women/18.jpg" alt="" />
          <p>Erica</p>
        </a>
      </li>
    </ul>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.videobar {
  background-color: #000;
}

.vb__title {
  font-size: 14px;
  color: #fff;
  margin-bottom: 12px;
}
.videobar__videos {
  display: flex;
  justify-content: space-between;
  .vb__video {
    a {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-decoration: none;
      img {
        width: 50px;
        height: 50px;
        border-radius: 50%;
        border: 1px solid #fff;
        margin-bottom: 4px;
      }
      p {
        color: #fff;
        font-size: 12px;
      }
    }
  }
}
</style>