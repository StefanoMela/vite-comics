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

/* 
@media (max-width: 768px) {
  .header__menu {
    position: absolute;
    top: 60px;
    left: 0;
    background-color: var(--menu-bg);
    width: 100%;
    height: 100vh;
    height: 0vh;
    overflow: hidden;
    transition: all 1s cubic-bezier(0.215, 0.61, 0.355, 1);
  }

  .header__menu li {
    width: 100%;
    border-bottom: 1px solid #444;
  }
  .menu-open .header__menu {
    height: 100vh;
    padding: 3%;
  }

  .icon-hamburger {
    height: 50px;
    width: 40px;
    margin-left: 20px;
    padding-top: 5px;
  }
  .icon-hamburger span {
    height: 2px;
    width: 30px;
    background: var(--menu-color);
    position: relative;
    display: block;
    margin-top: 11px;
    transition: all 0.2s cubic-bezier(0.215, 0.61, 0.355, 1);
  }

  .menu-open .icon-hamburger span:nth-child(1) {
    transform: rotate(45deg) translateY(9px);
  }
  .menu-open .icon-hamburger span:nth-child(2) {
    transform: rotate(-45deg) translateY(-9px);
  }

  .header__quick {
    display: flex;
    justify-content: flex-end;
    width: 50%;
  }
} */
</style>
