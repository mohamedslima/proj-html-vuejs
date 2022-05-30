<template>
  <header>
    <div class="header_info">
      <div>We have a 95% Successful Pass Rate</div>
      <div>
        <i class="fas fa-phone"></i>
        Give us a call to book your tuition! 1-800-555-555
        </div>
    </div>
    <div class="header_menu">
      <div>
        <img src="" alt="">
      </div>
      <div>

      </div>
      <div>

      </div>
    </div>
  </header>
</template>

<script>
export default {
    name: "AppHeader",
    data: function () {
      return {
        linksheader: [
          {
            url: "#",
            text: "HOME",
            new: false,
          },
          {
            url: "#",
            text: "ABOUT",
            new: false,
          },
          {
            url: "#",
            text: "PRICES",
            new: false,
          },
          {
            url: "#",
            text: "COURSES",
            new: true,
          },
          {
            url: "#",
            text: "LOCATIONS",
            new: false,
          },
          {
            url: "#",
            text: "BLOG",
            new: false,
          },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>

header {
  div.header_info {
    height: 40px;
    background-color: #484848;
    color: #a1a5ae;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    font-size: 0.8rem;
  }
}

</style>