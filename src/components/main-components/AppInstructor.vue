<template>
  <div class="instructor_container">
    <div class="instructor_text_container">
      <div class="instructor_text">
        <div>Your Instructors</div>
        <span>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt
          facere numquam amet soluta necessitatibus maxime iure id, magnam,
          deleniti possimus, temporibus quod distinctio.
        </span>
      </div>
      <div class="instructor_button">
        <button>MORE ABOUT US</button>
      </div>
    </div>
    <div></div>
  </div>
</template>

<script>
export default {
  name: "AppInstructor",
};
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

div.instructor_container {
  div.instructor_text_container {
    width: $general-content-width;
    margin: $general-content-margin;
    height: 250px;
    display: flex;
    align-items: center;
    justify-content:space-evenly;
    div.instructor_text {
        width: 60%;
        div {
            font-size: 2.3rem;
            margin-bottom: 2rem;
        }
        span {
            color: #3f4843cb;
            line-height: 2rem;
        }
    }
    div.instructor_button {
        button {
            margin-top: 1rem;
              background-color: $button-green-bg;
              color: $button-white-text;
              border: $button-border-green;
              font-weight: $button-weight-bold;
              cursor: $button-pointer;
              border-radius: $button-radius;
              padding: 0.5rem 7rem;
              &:hover {
                color: $button-green-text;
                background-color: $button-white-bg;
                transition: 0.5s;
              }
        }
    }
  }
}
</style>