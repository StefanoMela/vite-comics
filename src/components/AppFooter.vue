<script>
export default {
  data() {
    return {
      links: "",
    };
  },
};
</script>

<template>
  <div class="footer-container">
    <div class="fc_link_group">
        <ul class="fc_first_link_group">
          <li>First link</li>
          <li>Second Link</li>
          <li>Third Link</li>
          <li>Fourth Link</li>
        </ul>
        <ul class="fc_second_link_group">
          <li>First link</li>
          <li>Second Link</li>
          <li>Third Link</li>
          <li></li>
        </ul>
        <ul class="fc_third_link_group">
          <li>First link</li>
          <li>Second Link</li>
          <li>Third Link</li>
          <li>Fourth Link</li>
        </ul>
    </div>
    <div class="fc_img_overlay_container">
    </div>
    <div class="bottom-footer">
        <div class="fc_btn_container">
            <button>Call To Action</button>
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
    height: 400px;
    background-color: rgba(34, 32, 32, 0.915);

    padding-top: 30px;

    .fc_link_group{

        width: 40%;

        padding-left: 30px;

        display: flex;
        flex-direction: column;

    }

    .fc_img_overlay_container{

        width: 60%;
    }

    .bottom-footer{

        width: 100%;
        height: 120px;

        border: 1px solid red;

        display: flex;
        justify-content: space-around;
        align-items: center;

        .fc_social_icons_container>*{

            padding-inline: 1rem;
        }

    }
}
</style>