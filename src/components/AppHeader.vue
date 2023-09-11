<script>
export default {
  data() {
    return {
      Headerlinks: [
        {
          text: "CHARACTERS",
          href: "#",
          current: false,
        },
        {
          text: "COMICS",
          href: "#",
          current: true,
        },
        {
          text: "MOVIES",
          href: "#",
          current: false,
        },
        {
          text: "TV",
          href: "#",
          current: false,
        },
        {
          text: "GAMES",
          href: "#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          href: "#",
          current: false,
        },
        {
          text: "VIDEOS",
          href: "#",
          current: false,
        },
        {
          text: "FANS",
          href: "#",
          current: false,
        },
        {
          text: "NEWS",
          href: "#",
          current: false,
        },
        {
          text: "SHOP",
          href: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header class="header">
    <div class="header__content">
      <div class="header__logo__container">
        <a class="header__logo" href="#">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </a>
      </div>
      <div class="header__link__container">
        <ul v-for="link in Headerlinks" class="header__menu">
          <li>
            <a>{{ link.text }}</a>
          </li>
        </ul>
      </div>
      <div class="header__quick">
        <div class="icon-hamburger">
          <span></span>
          <span></span>
        </div>
      </div>
    </div>
  </header>
</template>

<style>
/* Menu */

.header__logo > img {
  max-width: 100px;
}

:root {
  --menu-bg: #1d1d1f;
}

.header {
  background-color: var(--menu-bg);
  width: 100%;
  padding-top: 30px;
}

.header__content {
  width: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-evenly;
  background-color: white;
  padding: 10px;
}

.header__logo,
.header__quick {
  display: flex;
  align-items: center;
  color: var(--menu-color);
}

.header__menu {
  display: inline-block;
}

.header__menu li a {
  color: var(--menu-color);
  opacity: 0.8;
  display: block;
  padding: 16px;
  font-size: 15px;
}

.header__menu li a:hover {

color: rgb(33, 33, 213);
border-bottom: 2px solid blue;
padding-bottom: 50px;


}
</style>
