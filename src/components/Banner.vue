<template>
  <div class="banner__container">
    <div class="banner__container__menu">
      <div class="menu--main">
        <li><a href="#">DANCE</a></li>
      </div>
      <div class="menu--submenu">
        <li><a href="#">ABOUT</a></li>
        <li><a href="#">BLOG</a></li>
        <li><a href="#">CONACT</a></li>
        <li><a href="#">REGISTER</a></li>
      </div>
    </div>
    <div class="banner__container__content">
      <img
        src="@/assets/main-dance.png"
        alt=""
        class="banner__container__content--image"
      />
      <div class="banner__container__content--text">
        <h1>Enjoy each step along the way.</h1>
        <h2>Learn to dance with style.</h2>
        <p>
          Learn More
          <button><img src="@/assets/arrow-right.png" alt="" /></button>
        </p>

        <div class="banner__container__content--socials">
          <p>FOLLOW US</p>
          <span class="line"></span>
          <img
            src="@/assets/fb-icon.png"
            alt=""
            class="banner__container__content--socialsImage"
          />
          <img
            src="@/assets/ig-icon.png"
            alt=""
            class="banner__container__content--socialsImage"
          />
          <img
            src="@/assets/tw-icon.png"
            alt=""
            class="banner__container__content--socialsImage"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.banner__container {
  padding: 130px 80px;
  background-image: linear-gradient(
    90deg,
    hsl(249deg 14% 10%) 0%,
    hsl(248deg 15% 10%) 22%,
    hsl(247deg 15% 11%) 31%,
    hsl(246deg 15% 12%) 38%,
    hsl(245deg 16% 13%) 45%,
    hsl(244deg 16% 13%) 52%,
    hsl(243deg 16% 14%) 60%,
    hsl(242deg 16% 15%) 70%,
    hsl(241deg 17% 15%) 82%,
    hsl(240deg 17% 16%) 100%
  );

  &__content {
    display: flex;
    justify-content: center;
    align-items: center;
    transform: translateY(-150px);
    &--image {
      max-width: 100%;
    }

    &--text {
      h1,
      h2,
      p {
        color: white;
        font-weight: 100;
        display: flex;
        gap: 20px;

        button {
          background: none;
          border: 1px solid white;
          border-radius: 10px;
          width: 30px;
          height: 30px;
        }
      }

      h1 {
        font-size: 2.5rem;
      }

      h2 {
        font-size: 60px;
        font-weight: 300;
      }

      p {
        font-size: 25px;
        text-transform: uppercase;
        font-weight: 400;
      }
    }

    &--socials {
      display: flex;
      gap: 45px;
      align-items: center;
      margin-top: 258px;
      .line {
        width: 50px;
        height: 2px;
        background: white;
        display: block;
      }
      img {
        width: 24px;
        height: 24px;
      }
    }
  }

  &__menu {
    font-weight: 600;
    display: flex;
    width: 100%;
    justify-content: space-around;
    align-items: center;
    gap: 200px;
    padding: 10px;

    .menu--main {
      margin-right: 30px;
      li {
        a {
          font-size: 50px;
        }
      }
    }

    li {
      list-style-type: none;

      a {
        font-size: 20px;
        text-decoration: none;
        color: #c0bfc4;
      }
    }

    .menu--submenu {
      gap: 20px;
      display: flex;
      letter-spacing: 0.15em;
      line-height: 30px;
    }
  }
}

li {
  a {
  }
}
</style>
