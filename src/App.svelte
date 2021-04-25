<script>
  import Typewriter from "svelte-typewriter";
</script>

<div class="parallax" />

<div class="container">
  <Typewriter loop>
    <h1>Elisa Giorgi</h1>
    <p>Software developer</p>
  </Typewriter>
</div>

<div class="parallax" />

<style>
  .container {
    height: 1000px;
    color: white;
    background-color: black;
    font-size: 50px;
    padding-top: 50px;
    text-align: center;
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

  /* Turn off parallax scrolling for tablets and phones. Increase the pixels if needed */
  @media only screen and (max-device-width: 1366px) {
    .parallax {
      background-attachment: scroll;
    }
  }
</style>
