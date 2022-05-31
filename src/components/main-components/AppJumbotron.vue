<template>
  <div class="jumbotron_container">
    <div class="jumbotron_presentation">
      <div class="jumbotron_text">
        <h1 class="jumbotron_title">Drive with Avada</h1>
        <h3 class="jumbotron_subtitle">
          We offer the finest driving tuition money can buy
        </h3>
      </div>
    </div>
    <div class="jumbotron_subscription">
      <div class="jumbotron_regi_width">
        <div class="jumbotron_info">
          <h2>Get Behind The Wheel</h2>
          <div class="jumbotron_left_text1">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptas
            voluptate esse vitae, reprehenderit consequatur. Lorem ipsum dolor,
            sit amet consectetur adipisicing elit. Voluptas voluptate esse
            vitae, reprehenderit consequatur.
          </div>
          <div class="jumbotron_left_text2">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Excepturi,
            vel minima doloremque numquam sequi ad deserunt laboriosam veniam
            possimus blanditiis rerum eum cumque a ullam libero at, sit et
            voluptatum! Lorem, ipsum dolor sit amet consectetur adipisicing
            elit. Excepturi, vel minima doloremque numquam sequi ad deserunt
            laboriosam veniam possimus blanditiis rerum eum cumque a ullam
            libero.
          </div>
        </div>
        <div class="jumbotron_registration">
          <div class="registration_card">
            <h4>First Lesson Free!</h4>
            <div class="text_registration">
              When you make a block booking with us your first lesson is
              included free.
            </div>
            <div class="input_container">
              <input type="text" placeholder="Your Name*" />
              <input type="text" placeholder="Email*" />
              <input type="text" placeholder="Telephone" />
              <input type="text" placeholder="Location" />
              <button>REQUEST A CALLBACK</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbotron",
};
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

div.jumbotron_container {
  div.jumbotron_presentation {
    background-image: url("../../assets/images/homepage-hero-background.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    height: 700px;
    display: flex;
    align-items: center;
    div.jumbotron_text {
      width: $general-content-width;
      margin: $general-content-margin;
      color: white;
      h1.jumbotron_title {
        font-size: 3rem;
        margin-bottom: 1rem;
      }
    }
  }
  div.jumbotron_subscription {
    div.jumbotron_regi_width {
      width: $general-content-width;
      margin: $general-content-margin;
      display: flex;
      justify-content: space-between;
      div.jumbotron_info {
        width: calc(100% / 2);
        line-height: 2.5rem;
        margin-top: 5rem;
        h2 {
          font-size: 2.3rem;
        }
        div.jumbotron_left_text1 {
          font-size: 1.2rem;
          color: $general-gray-color-text;
          margin: 2rem 0;
        }
        div.jumbotron_left_text2 {
          font-size: 0.9rem;
          color: $general-gray-color-text;
        }
      }
      div.jumbotron_registration {
        div.registration_card {
          position: relative;
          top: -40px;
          text-align: center;
          padding: 4rem 0.5rem;
          border-radius: 10px;
          box-shadow: 1px 4px 8px 0 rgba(0, 0, 0, 0.2);
          background-color: white;
          h4 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
          }
          div.text_registration {
            width: 80%;
            margin: 0 auto;
            line-height: 2rem;
          }
          div.input_container {
            input {
              display: block;
              width: 80%;
              margin: 30px auto;
              height: 40px;
              background-color: #e5e8eb59;
              border: 1px solid gray;
              border-radius: 5px;
            }
            button {
              margin-top: 1rem;
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
  }
}
</style>