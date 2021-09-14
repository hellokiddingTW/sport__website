<template>
  <div>
    <nav class="mb-3">
      <div
        class="
          n__list
          d-flex
          justify-content-between
          align-items-center
          py-2
          container
        "
      >
        <h1 class="nav__logo">
          <a href="#"><img src="../assets/sexySport.png" alt="" /></a>
        </h1>
        <div class="nav__profile d-flex flex-column align-items-center">
          <a href="#" class="nav__profile__btn">
            <span class="material-icons"> person_outline </span>
          </a>
          <div class="nav__profile__money">
            <p class="m-0 me-1">NT $1000.0</p>
            <span class="material-icons nav__profile__plusIcan"> add </span>
          </div>
        </div>
      </div>
      <ul class="nav__links container">
        <li class="n__link" @click="clicked = 'sport'">
          <a href="#" :class="{ clicked: clicked == 'sport' }">體育投注</a>
        </li>
        <li class="n__link" @click="clicked = 'inPlay'">
          <a href="#" :class="{ clicked: clicked == 'inPlay' }">走地盤</a>
        </li>
        <li class="n__link" @click="clicked = 'myBet'">
          <a href="#" :class="{ clicked: clicked == 'myBet' }">我的投注</a>
        </li>
        <li class="n__link" @click="clicked = 'contact'">
          <a href="#" :class="{ clicked: clicked == 'contact' }">聯絡我們</a>
        </li>
      </ul>
      <ul class="nav__dates container">
        <li
          v-for="date in dateAry"
          :key="date.id"
          class="n__date"
          @click="dateClicked = date.id"
          :class="{ clicked: dateClicked == date.id }"
        >
          <p class="m-0" v-if="today == date.dateNow">today</p>
          <p class="m-0" v-else>{{ date.monthNow }} {{ date.dateNow }}</p>
        </li>
      </ul>
      <ul class="nav__sports container">
        <li
          class="n__sport"
          @click="sportClick = 'basketball'"
          :class="{ clicked: sportClick == 'basketball' }"
        >
          <img src="https://i.imgur.com/4Rt6S7Y.png" alt="" class="mb-1" />
          <p class="fw-bold">籃球</p>
        </li>
        <li
          class="n__sport"
          @click="sportClick = 'soccer'"
          :class="{ clicked: sportClick == 'soccer' }"
        >
          <img src="https://i.imgur.com/RL8R90d.png" alt="" class="mb-1" />
          <p class="fw-bold">足球</p>
        </li>
        <li
          class="n__sport"
          @click="sportClick = 'tennis'"
          :class="{ clicked: sportClick == 'tennis' }"
        >
          <img src="https://i.imgur.com/MWsGcy0.png" alt="" class="mb-1" />
          <p class="fw-bold">網球</p>
        </li>
        <li
          class="n__sport"
          @click="sportClick = 'volleyball'"
          :class="{ clicked: sportClick == 'volleyball' }"
        >
          <img src="https://i.imgur.com/MDrygqF.png" alt="" class="mb-1" />
          <p class="fw-bold">排球</p>
        </li>
        <li
          class="n__sport"
          @click="sportClick = 'handball'"
          :class="{ clicked: sportClick == 'handball' }"
        >
          <img src="https://i.imgur.com/d7kDkV2.png" alt="" class="mb-1" />
          <p class="fw-bold">手球</p>
        </li>
        <li
          class="n__sport"
          @click="sportClick = 'tableTennis'"
          :class="{ clicked: sportClick == 'tableTennis' }"
        >
          <img src="https://i.imgur.com/wlPok7a.png" alt="" class="mb-1" />
          <p class="fw-bold">桌球</p>
        </li>
      </ul>
    </nav>
  </div>
</template>


<script>
export default {
  data() {
    return {
      clicked: "inPlay",
      today: "",
      dateAry: [],
      dateClicked: null,
      sportClick: "soccer",
    };
  },
  methods: {
    getDate(days) {
      let month = [
        "Jan",
        "Feb",
        "Mar",
        "Apr",
        "May",
        "Jun",
        "Jul",
        "Aug",
        "Sep",
        "Oct",
        "Nov",
        "Dec",
      ];

      this.today = new Date().getDate();
      this.dateClicked = new Date().getTime();
      for (let i = 0; i < days; i++) {
        let monthNow = month[new Date().getMonth()];
        let currentDate = new Date();
        currentDate.setDate(currentDate.getDate() + i);
        this.dateAry.push({
          monthNow,
          dateNow: currentDate.getDate(),
          id: currentDate.getTime(),
        });
        console.log(i);
        console.log(currentDate);
      }
    },
  },
  created() {
    this.getDate(5);
  },
};
</script>
<style lang="scss" scoped>
.fz-sm {
  font-size: 12px;
}

nav {
  background-color: #000;
}

.nav__profile__money {
  display: flex;
  text-align: right;
  align-items: center;
  color: grey;
  font-size: 12px;
  .nav__profile__plusIcan {
    color: #fff;
    font-size: 12px;
    font-weight: bold;
    margin-left: 0.025em;
    cursor: pointer;
  }
}

.nav__profile__btn {
  color: #fff;
  height: 20px;
  margin-top: 0.25rem;
  &:hover {
    color: #bebebe;
  }
  .material-icons {
    font-size: 20px;
  }
}

.nav__logo {
  img {
    width: 99px;
    height: 33px;
  }
}

.nav__links {
  display: flex;
  justify-content: space-between;
  background-color: #3c3c3c;

  .n__link {
    padding: 0.5rem 0.5rem 10px 0.5rem;
    a {
      color: #7b7b7b;
      font-weight: 700;
      position: relative;
      text-decoration: none;
      font-size: 14px;
      &::after {
        content: "";
        position: absolute;
        width: 0%;
        height: 1px;
        background-color: #fff;
        left: 0;
        bottom: -4px;
        transition: all 0.5s;
      }
      &:hover {
        color: #fff;
        &::after {
          width: 100%;
        }
        transition: all 0.5s;
      }
    }
    .clicked {
      color: #fff;
      &::after {
        content: "";
        position: absolute;
        width: 100%;
        height: 2px;
        background-color: #fff;
        left: 0;
        bottom: -4px;
      }
    }
  }
}

.nav__dates {
  display: flex;
  justify-content: space-between;
  color: #7b7b7b;
  font-size: 12px;
  font-weight: bold;
  .n__date {
    padding: 1rem 0.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    cursor: pointer;
    position: relative;
    &:hover {
      color: #cecece;
    }
  }
  .clicked {
    color: #fff;
    &::after {
      content: "";
      position: absolute;
      width: 100%;
      height: 2px;
      background-color: #fff;
      left: 0;
      bottom: 12px;
    }
  }
}

.nav__sports {
  display: flex;
  justify-content: space-between;
  .n__sport {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 0.5rem 14px;
    cursor: pointer;
    img {
      width: 28px;
      height: 28px;
    }
    p {
      margin-bottom: 0px;
      font-size: 12px;
      color: #6c6c6c;
    }
  }
  .clicked {
    border: 1px solid #fff;
    border-radius: 0.5rem;
    p {
      color: #fff;
    }
  }
}

@media (min-width: 576px) {
}
</style>