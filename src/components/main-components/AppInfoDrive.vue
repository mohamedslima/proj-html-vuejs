<template>
  <div class="app_info_container">
    <div class="info_drive_contact">
      <div class="info_app_width">
        <div class="info_text_contact">
          <h2>Start Learning To Drive Today</h2>
          <div>Give us a call to schedule your first driving lesson</div>
        </div>
        <div class="info_number_contact">
          <i class="fas fa-phone"></i>
          1-800-555-555
        </div>
      </div>
    </div>
    <div class="app_course_info">
      <div class="course_app_width">
        <div class="course_card_container">
          <div class="course_card">
            <div class="new_box_card">NEW</div>
            <div class="course_card_text">
              <h3>Courses</h3>
              <div>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste
                necessitatibus cumque assumenda in animi, vitae cum corporis
                repellat quia incidunt odio autem.
              </div>
              <button>COURSE INFORMATION</button>
            </div>
          </div>
        </div>
        <div class="course_plus_info_container">
          <div class="plus_info_card">
            <img
              src="../../assets/images/courses-passplus.jpg"
              alt="img-info-1"
            />
            <span>Pass Plus</span>
            <button>LEARN MORE</button>
          </div>
          <div class="plus_info_card">
            <img
              src="../../assets/images/courses-passplus.jpg"
              alt="img-info-2"
            />
            <span>Intensive Course</span>
            <button>LEARN MORE</button>
          </div>
          <div class="plus_info_card">
            <img
              src="../../assets/images/courses-passplus.jpg"
              alt="img-info-3"
            />
            <span>Instructors</span>
            <button>LEARN MORE</button>
          </div>
        </div>
      </div>
      <div class="rating_container">
        <div class="rating_card">
          <div class="circle_rating first">95%</div>
          <div class="rating_text">PASS RATE</div>
        </div>
        <div class="rating_card">
          <div class="circle_rating second">100%</div>
          <div class="rating_text">REFFERAL RATE</div>
        </div>
        <div class="rating_card">
          <div class="circle_rating third">0%</div>
          <div class="rating_text">ACCIDENT RATE</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppInfoDrive",
};
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

div.app_info_container {
  div.info_drive_contact {
    background-image: url("../../assets/images/horizontal-cta-background.jpg");
    background-size: cover;
    height: 300px;
    div.info_app_width {
      width: $general-content-width;
      margin: $general-content-margin;
      color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-top: 100px;
      div.info_text_contact {
        line-height: 2.5rem;
        h2 {
          font-size: 2.3rem;
        }
        div {
          font-weight: bold;
        }
      }
      div.info_number_contact {
        font-size: 2rem;
      }
    }
  }
  div.app_course_info {
    div.course_app_width {
      width: $general-content-width;
      margin: $general-content-margin;
      display: flex;
      div.course_card_container {
        div.course_card {
          background-color: white;
          width: 25rem;
          height: 25rem;
          text-align: center;
          border-radius: 20px;
          box-shadow: 1px 4px 8px 0 rgba(0, 0, 0, 0.2);
          position: relative;
          top: -30px;
          div.new_box_card {
            background-color: #85b680;
            text-align: center;
            color: white;
            font-weight: bold;
            padding-top: 0.5rem;
            font-size: 0.8rem;
            width: 4rem;
            height: 2rem;
            border-radius: 1rem 0 1rem 0;
          }
          div.course_card_text {
            h3 {
              font-size: 1.8rem;
            }
            div {
              width: 90%;
              margin: 2rem auto;
              line-height: 1.8rem;
              color: $general-gray-color-text;
            }
            button {
              margin-top: 1rem;
              background-color: $button-green-bg;
              color: $button-white-text;
              border: $button-border-green;
              font-size: 1rem;
              font-weight: $button-weight-bold;
              cursor: $button-pointer;
              border-radius: $button-radius;
              padding: 0.5rem 1.5rem;
              &:hover {
                color: $button-green-text;
                background-color: $button-white-bg;
                transition: 0.5s;
              }
            }
          }
        }
      }
      div.course_plus_info_container {
        display: flex;
        justify-content: space-between;
        margin-left: 2.5rem;
        div.plus_info_card {
          width: calc(100% / 3);
          height: 40px;
          margin-top: 5rem;
          text-align: center;
          img {
            width: 13rem;
          }
          span {
            font-size: 1rem;
            color: #7f9ea8;
            font-weight: bold;
            line-height: 2rem;
          }
          button {
            border: 2px solid #7f9ea8;
            display: block;
            margin-left: 3.5rem;
            margin-top: 0.5rem;
            background-color: white;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            color: #7f9ea8;
            &:hover {
              border: 2px solid #85b680;
              color: #85b680;
              transition: 0.5s;
            }
          }
        }
      }
    }
    div.rating_container {
      display: flex;
      justify-content: space-evenly;
      width: $general-content-width;
      margin: $general-content-margin;
      div.rating_card {
          margin-top: 3rem;
        width: calc(100% / 3 - 15px);
        height: 28rem;
        border-radius: 10px;
        border-top: 6px solid #85b680;
        box-shadow: 2px 4px 8px 0 rgba(0, 0, 0, 0.2);
        div.circle_rating {
          height: 200px;
          width: 200px;
          margin: 0 auto;
          border-radius: 50%;
          border: 8px solid #e5e8eb;
          text-align: center;
          padding: 70px;
          color: #3f4843c0;
          font-size: 2rem;
          margin-top: 3rem;
        }
        div.circle_rating.first {
          border-top: 8px solid #85b680;
          border-right: 8px solid #85b680;
          border-bottom: 8px solid #85b680;
        }
        div.circle_rating.second {
          border: 8px solid #85b680;
          padding: 70px 60px;
        }
        div.rating_text {
          color: #3f4843c0;
          font-weight: bold;
          text-align: center;
          margin-top: 2rem;
        }
      }
    }
  }
}
</style>