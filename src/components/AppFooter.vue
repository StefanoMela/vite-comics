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
            <li class="list-title" style="color:white; font-weight: bold;">DC COMICS</li>
            <li 
            v-for="(link, index) in footerLinks"
            :key="index"
            >
            {{link.text}}</li>
          </ul>
          <ul class="fc_second_link_group">
            <li class="list-title" style="color:white; font-weight: bold;">DC COMICS</li>
            <li 
            v-for="(link, index) in shopLinks"
            :key="index"
            >
            {{ link.text}}</li>
          </ul>
          <ul class="fc_third_link_group">
            <li class="list-title" style="color:white; font-weight: bold;">DC COMICS</li>
            <li 
            v-for="(link, index) in dcLinks"
            :key="index"
            >
            {{ link.text }}</li>
          </ul>
      </div>
      <div class="fc_img_overlay_container">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    <div class="bottom-footer">
        <div class="fc_btn_container">
            <button>Sign Up Now</button>
        </div>
        <div class="fc_social_icons_container">
            <span>FOLLOW US</span>
            <i>iconeSocial</i>
            <i>iconeSocial</i>
            <i>iconeSocial</i>
            <i>iconeSocial</i>
            <i>iconeSocial</i>
        </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-container{

    width: 100%;
    max-height: 400px;
    background-color: rgba(34, 32, 32, 0.915);

    .footer__divider{

      display: flex;
      justify-content: space-between;
      background-image: url(../assets/img/footer-bg.jpg);
    }

    .fc_link_group{

        width: 40%;

        padding-left: 30px;

        display: flex;
        flex-direction: column;
        flex-wrap: wrap;

    }

    .fc_img_overlay_container{

        width: 60%;
        img{
            max-height: 400px;
        }
    }

    .bottom-footer{

        width: 100%;
        height: 120px;

        display: flex;
        justify-content: space-around;
        align-items: center;

        .fc_social_icons_container>*{

            padding-inline: 1rem;
        }

    }
}
</style>