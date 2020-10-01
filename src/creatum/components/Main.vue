<template>
  <div class="main">
    <div class="main__wrapp">
      <div class="content__wrapp">
        <p class="main__content">
          We create <b> brands </b>and craft <br />
          beautiful digital <br />
          <b> experiences</b>
        </p>
        <p class="main__content--right">
          We help <b> startups</b> and <br />
          <b> companies</b> with design and <br />
          marketing
        </p>

        <div class="main__poly">
          <p class="third__signature signature">
            Design
          </p>
          <p>
            <svg
              class="poly__img"
              width="176"
              height="154"
              viewBox="0 0 176 154"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M88.089 2L174.692 152H1.48645L88.089 2Z"
                stroke="#272727"
                stroke-width="2.5"
                stroke-linejoin="round"
              />
            </svg>
          </p>

          <p class="poly poly__sec">
            <svg
              class="poly__img"
              width="176"
              height="154"
              viewBox="0 0 176 154"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M88.089 2L174.692 152H1.48645L88.089 2Z"
                stroke="#272727"
                stroke-width="2.5"
                stroke-linejoin="round"
              />
            </svg>
          </p>

          <p class="poly poly__third">
            <svg
              class="poly__img"
              width="176"
              height="154"
              viewBox="0 0 176 154"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M88.089 2L174.692 152H1.48645L88.089 2Z"
                stroke="#272727"
                stroke-width="2.5"
                stroke-linejoin="round"
              />
            </svg>
          </p>
          <p class="first__signature signature">
            Marketing
          </p>
          <p class="second__signature signature">Websites</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {
      isActive: false
    };
  }
};
</script>

<style lang="scss" scoped>
.main {
  background-color: #fcfbf7;
}
.main__wrapp {
  margin: 0 auto;
  //background-color: aqua;
  max-width: 1200px;
}
.content__wrapp {
  display: flex;
  justify-content: space-between;
}
.main__content {
  text-align: justify;
  font-family: Montserrat, sans-serif;
  font-size: 24px;
  order: 1;
  padding-top: 150px;
  &--right {
    font-family: Montserrat, sans-serif;
    font-size: 24px;
    padding-top: 150px;
    text-align: right;
    order: 3;
  }
}
.main__poly {
  position: relative;
  order: 2;
  //opacity: 0.3;
  // margin: 0 auto;
}
.poly {
  &:hover {
    cursor: pointer;
    //background-color: #fff;
  }
}
.poly__img {
  fill: antiquewhite;
  color: red;
  opacity: 0.1;
}
.poly__img:hover {
  transition: 3s;
  opacity: 1;
  stroke-linejoin: round;
  stroke: #050814;
  fill: #4c61bd;
}

.poly__sec {
  position: relative;
  bottom: 21px;
  left: -88px;
}
.poly__third {
  position: relative;
  bottom: 195px;
  left: 88px;
}
.signature {
  font-family: Anglecia Pro Title, sans-serif;
  font-style: italic;
  font-size: 28px;
  font-weight: 700;
}
.first__signature {
  display: inline-block;
  position: relative;
  left: -199px;
  bottom: 193px;
}

.second__signature {
  display: inline-block;
  position: relative;
  right: -199px;
  bottom: 193px;
}
</style>
