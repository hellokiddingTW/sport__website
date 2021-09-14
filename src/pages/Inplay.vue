<template>
  <div>
    <div class="inplay">
      <div
        class="inplay__header d-flex text-white align-items-center container"
      >
        <h3 class="inplay__header__title">足球</h3>
        <div class="inplay__header__filter ms-auto fw-bold">
          <span class="material-icons"> filter_alt </span>
        </div>
      </div>
      <div class="inplay__league">
        <h4 class="leauge__name m-0">英國超級聯賽</h4>
        <div class="inplay__games mb-3">
          <div class="content__time d-flex text-white p-2">
            <p class="m-0 me-3">上半場</p>
            <p class="fw-bold m-0">0:00</p>
            <div class="content__more ms-auto">
              <span class="fw-bold">+65</span>
              <span class="material-icons"> chevron_right </span>
            </div>
          </div>
          <div class="inplay__league__content d-flex py-3">
            <div class="content__team px-1">
              <div>
                <div class="d-flex align-items-center mb-1">
                  <img
                    class="content__team__logo"
                    src="https://i.imgur.com/LFFOf5s.png"
                    alt=""
                  />
                  <span class="ms-1">水晶宮</span>
                  <p class="fw-bold mb-0 ms-auto">0</p>
                </div>
                <div class="d-flex align-items-center mb-1">
                  <img
                    class="content__team__logo"
                    src="https://i.imgur.com/IDt7qXR.png"
                    alt=""
                  />
                  <span class="ms-1">熱刺</span>
                  <p class="fw-bold mb-0 ms-auto">0</p>
                </div>
              </div>
              <div class="content__team__data ms-3">
                <div class="d-flex">
                  <a href="#"
                    ><span class="material-icons me-1"> smart_display </span>
                  </a>
                  <a href="">
                    <span class="material-icons"> insert_chart </span>
                  </a>
                </div>
              </div>
            </div>
            <div class="inplay__bet px-1">
              <div class="bet__single">
                <h4 class="text-center">全場獨贏</h4>
                <div class="text-center bet__btn single--bet">
                  <p>主勝</p>
                  <p>2.25</p>
                </div>
                <div class="text-center bet__btn single--bet">
                  <p>客勝</p>
                  <p>2.25</p>
                </div>
                <div class="text-center bet__btn single--bet">
                  <p>和局</p>
                  <p>2.25</p>
                </div>
              </div>
              <div class="bet__handicap">
                <h4 class="text-center">全場讓分</h4>
                <div class="text-center bet__btn handicap--btn">
                  <p>-1.5</p>
                  <p>1.95</p>
                </div>
                <div class="text-center bet__btn handicap--btn">
                  <p>+1.5</p>
                  <p>1.95</p>
                </div>
              </div>
              <div class="content__score">
                <h4 class="text-center">全場大小</h4>
                <div class="text-center bet__btn score--btn">
                  <p>大 2.5</p>
                  <p>1.95</p>
                </div>
                <div class="text-center bet__btn score--btn">
                  <p>小 2.5</p>
                  <p>1.95</p>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="inplay__games mb-3">
          <div class="content__time d-flex text-white p-2">
            <p class="m-0 me-3">下半場</p>
            <p class="fw-bold m-0">0:00</p>
            <div class="content__more ms-auto">
              <span class="fw-bold">+65</span>
              <span class="material-icons"> chevron_right </span>
            </div>
          </div>
          <div class="content__team p-2 d-flex flex-row w-100">
            <div class="d-flex align-items-center">
              <img
                class="content__team__logo"
                src="https://i.imgur.com/dbpmLqT.png"
                alt=""
              />
              <span class="ms-1">曼聯</span>
            </div>
            <div>
              <span>0 </span>
              <span>-</span>
              <span> 0</span>
            </div>
            <div class="d-flex align-items-center flex-row-reverse">
              <img
                class="content__team__logo"
                src="https://i.imgur.com/ettIZQp.png"
                alt=""
              />
              <span class="me-1">紐卡索</span>
            </div>
          </div>
          <div class="inplay__league__content d-flex pb-3">
            <div class="bet__video px-1">
              <img
                src="https://i.imgur.com/IBMgUUD.png"
                alt=""
                class="videoBar"
              />
              <span class="material-icons videoIcon"> videocam </span>
              <img
                src="https://images.chinatimes.com/newsphoto/2020-12-29/656/20201229002840.jpg"
                alt=""
              />
            </div>
            <div class="inplay__bet px-1">
              <div class="bet__single">
                <h4 class="text-center">全場獨贏</h4>
                <div class="text-center bet__btn">
                  <p>主勝</p>
                  <p>2.25</p>
                </div>
                <div class="text-center bet__btn">
                  <p>客勝</p>
                  <p>2.25</p>
                </div>
                <div class="text-center bet__btn">
                  <p>和局</p>
                  <p>2.25</p>
                </div>
              </div>
              <div class="bet__handicap">
                <h4 class="text-center">全場讓分</h4>
                <div class="text-center bet__btn handicap--btn">
                  <p>-1.5</p>
                  <p>1.95</p>
                </div>
                <div class="text-center bet__btn handicap--btn">
                  <p>+1.5</p>
                  <p>1.95</p>
                </div>
              </div>
              <div class="content__score">
                <h4 class="text-center">全場大小</h4>
                <div class="text-center bet__btn score--btn">
                 <p>大 2.5</p>
                  <p>1.95</p>
                </div>
                <div class="text-center bet__btn score--btn">
                 <p>小 2.5</p>
                  <p>1.95</p>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="inplay__games mb-3">
          <div class="content__time d-flex text-white p-2">
            <p class="m-0 me-3">下半場</p>
            <p class="fw-bold m-0">0:00</p>
            <div class="content__more ms-auto">
              <span class="fw-bold">+65</span>
              <span class="material-icons"> chevron_right </span>
            </div>
          </div>
          <div class="content__team p-2 d-flex flex-row w-100">
            <div class="d-flex align-items-center">
              <img
                class="content__team__logo"
                src="https://i.imgur.com/dbpmLqT.png"
                alt=""
              />
              <span class="ms-1">曼聯</span>
            </div>
            <div>
              <span>0 </span>
              <span>-</span>
              <span> 0</span>
            </div>
            <div class="d-flex align-items-center flex-row-reverse">
              <img
                class="content__team__logo"
                src="https://i.imgur.com/ettIZQp.png"
                alt=""
              />
              <span class="me-1">紐卡索</span>
            </div>
          </div>
          <div class="inplay__league__content d-flex pb-3">
            <div class="bet__video px-1">
              <img
                src="https://i.imgur.com/gs7CWog.png"
                alt=""
                class="audioBar"
              />
              <span class="material-icons videoIcon"> volume_up </span>
              <img
                src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcT6_zQ1pRl4BFo5UveJ32PaVP2_CTGamwwJYw&usqp=CAU"
                alt=""
              />
            </div>
            <div class="inplay__bet px-1">
              <div class="bet__single">
                <h4 class="text-center">全場獨贏</h4>
                <div class="text-center bet__btn single--btn">
                  <p>主勝</p>
                  <p>2.25</p>
                </div>
                <div class="text-center bet__btn single--btn">
                 <p>客勝</p>
                  <p>2.25</p>
                </div>
                <div class="text-center bet__btn">
                  <p>和局</p>
                  <p>2.25</p>
                </div>
              </div>
              <div class="bet__handicap">
                <h4 class="text-center">全場讓分</h4>
                <div class="text-center bet__btn handicap--btn">
                  <p>-1.5</p>
                  <p>1.95</p>
                </div>
                <div class="text-center bet__btn handicap--btn">
                  <p>+1.5</p>
                  <p>1.95</p>
                </div>
              </div>
              <div class="content__score">
                <h4 class="text-center">全場大小</h4>
                <div class="text-center bet__btn score--btn">
                 <p>大 2.5</p>
                 <p class="oddsDown">1.95</p>
                </div>
                <div class="text-center bet__btn score--btn">
                 <p>小 2.5</p>
                 <p class="oddsUp"> 1.95</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>

<style lang="scss" scoped>
.inplay__header__title {
  font-size: 20px;
  font-weight: bold;
}

.inplay__header__filter {
  font-size: 12px;
  span {
    font-size: 12px;
  }
}

.leauge__name {
  font-size: 16px;
  color: #e0e0e0;
  background-color: #585858;
  padding: 0.5rem 1rem;
}

.content__team {
  color: #cecece;
  width: 33%;
  font-size: 14px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  img {
    width: 30px;
    height: 30px;
  }
}

.content__team__data {
  span {
    color: #e0e0e0;
  }
}
.content__more {
  display: flex;
  align-items: center;
  // justify-content: center;
}

.inplay__bet {
  width: 66%;
  display: flex;
  justify-content: space-around;
  h4 {
    font-size: 12px;
    color: #2894ff;
    padding: 0.5rem 10px;
    border-radius: 0.25rem;
    background-color: #adadad33;
    margin: 0;
  }

  p {
    margin: 0;
  }
  .bet__btns {
    display: flex;
    flex-direction: column;
    align-items: center;

    .handicap--btn,
    .score--btn {
      height: 67px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
  }
  .bet__single {
    display: grid;
    width: 32%;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 2fr 2fr 2fr;
    gap: 4px 4px;
  }
  .bet__handicap,
  .content__score {
    display: grid;
    width: 32%;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr 3fr 3fr;
    gap: 4px 4px;
  }
  .bet__btn {
    background-color: #d0d0d033;
    border-radius: 0.25rem;
    padding: 0.25rem 0;
    width: 100%;
    font-size: 12px;
    color: #2894ff;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    &:hover{
        background-color: #FCFCFC;
        color:#0000E3;
        font-weight: bold;
    }
    .oddsDown{
        color:green;
        &::before{
            content:'▼';
            position: relative;
            color:green;
            margin-right: 0.25rem;
        }
    }
    .oddsUp{
         color:red;
        &::before{
            content:'▲';
            position: relative;
            color:red;
            margin-right: 0.25rem;
        }
    }
  }
}

.content__time {
  border-top: 1px solid #fff;
  border-bottom: 1px solid #fff;
}

.bet__video {
  display: grid;
  width: 33%;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr;
  position: relative;
  &::after {
    content: "點擊觀看";
    position: absolute;
    width: 100%;
    background-color: #000000cc;
    color: #cecece;
    font-weight: bold;
    text-align: center;
    bottom: 0;
    font-size: 12px;
  }
  &::before {
    content: "Erica";
    position: absolute;
    width: 100%;
    background-color: #00000080;
    font-weight: 700;
    text-align: center;
    color: #ff79bc;
    bottom: 18px;
  }
  img {
    height: 222px;
    width: 100%;
    object-fit: cover;
    border-radius: 0.5rem;
  }
  .videoIcon {
    position: absolute;
    right: 0.5rem;
    color: #f00078;
  }
  .audioBar {
    position: absolute;
    top: 0.25rem;
    left: 0.5rem;
    width: 53px;
    height: 15px;
  }

  .videoBar {
    position: absolute;
    top: 0.25rem;
    left: 0.5rem;
    width: 53px;
    height: 15px;
  }
}

@media(min-width:576px){
    .bet__video{
        img{
            height:auto
        }
    }
}
</style>