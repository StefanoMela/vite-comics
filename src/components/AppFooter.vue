<script>
export default {
  data() {
    return {
      footerLinks: [
        {
          text: "Characters",
          href: "#",
          current: false,
        },
        {
          text: "Comics",
          href: "#",
          current: false,
        },
        {
          text: "Movies",
          href: "#",
          current: false,
        },
        {
          text: "TV",
          href: "#",
          current: false,
        },
        {
          text: "Games",
          href: "#",
          current: false,
        },
        {
          text: "Collectibles",
          href: "#",
          current: false,
        },
        {
          text: "Videos",
          href: "#",
          current: false,
        },
        {
          text: "News",
          href: "#",
          current: false,
        },
      ],

      shopLinks: [
        {
          text: "Shop DC",
          href: "#",
          current: false,
        },
        {
          text: "Shop DC Collectibles",
          href: "#",
          current: false,
        },
      ],

      dcLinks: [
        {
          text: "Terms Of Use",
          href: "#",
          current: false,
        },
        {
          text: "Privacy policy (New)",
          href: "#",
          current: false,
        },
        {
          text: "Ad Choices",
          href: "#",
          current: false,
        },
        {
          text: "Advertising",
          href: "#",
          current: false,
        },
        {
          text: "Jobs",
          href: "#",
          current: false,
        },
        {
          text: "Subscriptions",
          href: "#",
          current: false,
        },
        {
          text: "Talent Workshops",
          href: "#",
          current: false,
        },
        {
          text: "CPSC Certificates",
          href: "#",
          current: false,
        },
        {
          text: "Ratings",
          href: "#",
          current: false,
        },
        {
          text: "Shop Help",
          href: "#",
          current: false,
        },
        {
          text: "Contact Us",
          href: "#",
          current: false,
        },
      ],

      sitesLinks: [
        {
          text: "DC",
          href: "#",
          current: false,
        },
        {
          text: "MAD Magazine",
          href: "#",
          current: false,
        },
        {
          text: "DC Kids",
          href: "#",
          current: false,
        },
        {
          text: "DC Universe",
          href: "#",
          current: false,
        },
        {
          text: "DC Power Visa",
          href: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <div class="footer-container">
    <div class="footer__divider">
      <div class="fc_link_group">
        <ul class="fc_first_link_group">
          <li class="list-title" style="color: white; font-weight: bold">
            DC COMICS
          </li>
          <li v-for="(link, index) in footerLinks" :key="index">
            {{ link.text }}
          </li>
        </ul>
        <ul class="fc_second_link_group">
          <li class="list-title" style="color: white; font-weight: bold">
            SHOP
          </li>
          <li v-for="(link, index) in shopLinks" :key="index">
            {{ link.text }}
          </li>
        </ul>
        <ul class="fc_third_link_group">
          <li class="list-title" style="color: white; font-weight: bold">DC</li>
          <li v-for="(link, index) in dcLinks" :key="index">
            {{ link.text }}
          </li>
        </ul>
        <ul class="fc_fourth_link_group">
          <li class="list-title" style="color: white; font-weight: bold">
            SITES
          </li>
          <li v-for="(link, index) in sitesLinks" :key="index">
            {{ link.text }}
          </li>
        </ul>
      </div>
      <div class="fc_img_overlay_container">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
    </div>
    <div class="bottom-footer">
      <div class="fc_btn_container">
        <button class="call__to__action__button">Sign Up Now</button>
      </div>
      <div class="fc_social_icons_container">
        <span class="hl-text">FOLLOW US</span>
        <img src="../assets/img/footer-facebook.png" alt="" />
        <img src="../assets/img/footer-twitter.png" alt="" />
        <img src="../assets/img/footer-youtube.png" alt="" />
        <img src="../assets/img/footer-pinterest.png" alt="" />
        <img src="../assets/img/footer-periscope.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-container {
  width: 100%;
  background-image: url(../assets/img/footer-bg.jpg);
  padding-top: 2rem;
  position: relative;

  .fc_link_group {
    display: flex;
    flex-direction: row;
    gap: 1.5rem;
    padding-left: 2rem;

    color: #72787c;
  }

  .fc_img_overlay_container {
    overflow: hidden;
    img {
      max-width: 450px;
      position: absolute;
      top: -85px;
      right: 85px;
    }
  }

  .bottom-footer {
    width: 100%;
    background-color: #303030;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 1.5rem;

    .fc_social_icons_container {
      display: flex;
      align-items: center;
    }
    .fc_social_icons_container > * {
      padding-inline: .7rem;
    }

    .call__to__action__button {
      color: white;
      background-color: transparent;
      text-transform: uppercase;
      padding: 1rem;
      border: 1px solid #0082f9;
    }

    .hl-text {
      color: #0082f9;
      font-size: larger;
    }
  }
}
</style>
