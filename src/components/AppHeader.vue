<script>
export default {
  data() {
    return {
      headerlinks: [
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
          href: "www.google.com",
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
  <div class="header">
    <div class="header__content">
      <div class="header__logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="header__links">
        <ul>
          <li v-for="(link, index) in headerlinks"><a :href="href">{{ link.text }}</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss">

.header {

  width: 100%;
  padding: .8rem;
}

.header__content {

  display: flex;
  justify-content: space-evenly;
  align-items: center;

}
.header__logo img {
  max-width: 60px;
}

.header__links {
  li {
  
    display: inline-block;
    padding-inline: .5rem;
  } 
  
  li>a:hover {

  color: blue;
  padding-bottom: 8px;
  border-bottom: 5px solid blue;
}
}
</style>
