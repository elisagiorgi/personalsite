<script>
</script>

<div class="parallax">
  <div class="animated-title">
    <div class="text-top">
      <div>
        <span> It’s fine to celebrate success</span>
        <span>but it is more important to heed </span>
        <span> the lessons of failure.</span>
      </div>
    </div>
    <div class="text-bottom">
      <div>Bill Gates.</div>
    </div>
  </div>
</div>

<div class="container" />

<div class="parallax image2" />

<style>
  .container {
    height: 500px;
    background-color: black;
    padding-top: 50px;
    text-align: center;
    font-size: 40px;
    padding-top: 50px;
    text-align: center;
    color: white;
  }
  .parallax {
    /* The image used */
    background-image: url("../images/mountains.jpg");

    /* Full height */
    height: 100%;

    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  .image2 {
    background-image: url("../images/fire.jpg");
  }

  /* Turn off parallax scrolling for tablets and phones. Increase the pixels if needed */
  @media only screen and (max-device-width: 1366px) {
    .parallax {
      background-attachment: scroll;
    }
  }
  @import url("https://fonts.googleapis.com/css?family=Roboto:700");
  @keyframes showTopText {
    0% {
      transform: translate3d(0, 100%, 0);
    }
    40%,
    60% {
      transform: translate3d(0, 60%, 0);
    }
    100% {
      transform: translate3d(0, 0, 0);
    }
  }
  @keyframes showBottomText {
    0% {
      transform: translate3d(0, -100%, 0);
    }
    100% {
      transform: translate3d(0, 0, 0);
    }
  }
  .animated-title {
    color: #222;
    font-family: "Rubik", sans-serif;
    height: 100vh;
    left: 50%;
    position: absolute;
    top: 40vh;
    transform: translate(-50%, -50%);
    width: 90vw;
    font-size: 6vmin;
  }
  .animated-title > div {
    height: 50%;
    overflow: hidden;
    position: absolute;
    width: 100%;
  }
  .animated-title > div div {
    padding: 2vmin 0;
    position: absolute;
  }
  .animated-title > div div span {
    display: block;
    text-align: left;
  }

  .animated-title > div.text-top div {
    animation: showTopText 1s;
    animation-delay: 0.5s;
    animation-fill-mode: forwards;
    bottom: 0;
    transform: translate(0, 100%);
  }

  .animated-title > div.text-bottom {
    bottom: 0;
  }
  .animated-title > div.text-bottom div {
    animation: showBottomText 0.5s;
    animation-direction: alternate;
    animation-delay: 1.75s;
    animation-fill-mode: forwards;
    top: 0;
    transform: translate(0, -100%);
  }
</style>
