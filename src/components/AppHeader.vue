<template>
  <header>
    <div class="header_info">
      <div class="header_info_width">
        <div>We have a 95% Successful Pass Rate</div>
        <div>
          <i class="fas fa-phone"></i>
          Give us a call to book your tuition! 1-800-555-555
        </div>
      </div>
    </div>
    <div class="header_menu">
      <div class="header_menu_width">
        <div class="image_header_container">
          <img
            src="../assets/images/avada-drivers-logo-2x-300x58.png"
            alt="header-image-logo"
          />
        </div>
        <div class="header_list">
          <ul>
            <li
              v-for="(item, index) in linksHeader"
              :key="index"
              :class="{ active: item.active }"
            >
              <a href="#" :class="{ active: item.active }"> {{ item.text }}</a>
              <span class="new_box" :class="{ new: item.new }">NEW</span>
            </li>
          </ul>
        </div>
        <div class="header_button_container">
          <button class="header_button">BOOK NOW</button>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      linksHeader: [
        {
          url: "#",
          text: "HOME",
          active: false,
          new: false,
        },
        {
          url: "#",
          text: "ABOUT",
          active: false,
          new: false,
        },
        {
          url: "#",
          text: "PRICES",
          active: false,
          new: false,
        },
        {
          url: "#",
          text: "COURSES",
          active: false,
          new: true,
        },
        {
          url: "#",
          text: "LOCATIONS",
          active: false,
          new: false,
        },
        {
          url: "#",
          text: "BLOG",
          active: false,
          new: false,
        },
      ],
    };
  },
  methods: {
    isActive: function (index) {
      this.linksHeader.forEach((item, index) => {
        this.linksHeader[index].active = false;
      });
      this.linksHeader[index].active = !this.linksHeader[index].active;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header {
  div.header_info {
    height: 40px;
    background-color: #484848;
    color: #a1a5ae;
    font-size: 0.8rem;
    display: flex;
    align-items: center;
    div.header_info_width {
      width: $general-content-width;
      margin: $general-content-margin;
      display: flex;
      justify-content: space-between;
    }
  }
  div.header_menu {
    height: 110px;
    background-color: #48484860;
    display: flex;
    // position: fixed;
    top: 0;
    width: 100%;
    padding: 70px 0;
    div.header_menu_width {
      width: $general-content-width;
      margin: $general-content-margin;
      display: flex;
      justify-content: space-between;
      align-items: center;

      div.image_header_container {
        img {
          width: 70%;
        }
      }
      // styling list
      div.header_list {
        ul {
          list-style: none;
          display: flex;
          li {
            margin-right: 2rem;
            display: flex;
            &.active,
            &:hover {
              border-bottom: 3px solid #85b680;
              color: #85b680;
              padding-bottom: 0.6rem;
              transition: 0.5s;
            }
            a {
              text-decoration: none;
              color: white;
              font-weight: bold;
              &.active,
              &:hover {
                color: #85b680;
                transition: 0.5s;
              }
            }
            span.new_box {
              display: none;
              background-color: #85b680;
              color: white;
              font-size: 0.8rem;
              font-weight: bold;
              padding: 0.2rem;
              margin-left: 0.5rem;
              border-radius: 0.2rem;
              &.new {
                display: block;
              }
            }
          }
        }
      }
      // Button styling css set
      div.header_button_container {
        button.header_button {
          background-color: $button-green-bg;
          color: $button-white-text;
          border: $button-border-green;
          font-weight: $button-weight-bold;
          cursor: $button-pointer;
          border-radius: $button-radius;
          padding: 0.8rem 1.5rem;
          &:hover {
            color: $button-green-text;
            background-color: $button-white-bg;
            transition: 0.5s;
          }
        }
      }
    }
  }
}
</style>