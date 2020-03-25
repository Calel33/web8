<template>
  <div class="about">
    <title>Home</title>
    <Navbar />
    <br />
    <h1 class="display-3">

      Non-Custodial Wallets
    </h1>

    <img
      style="width:50%;"
      class="logo"
      alt="anansiweb logo"
      src="../static/anamsiweb new logo.png"
    />

    <br />
    <br />

    <br />

    <cc />
  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
export default {
  name: "Abouta",
  components: {
    Navbar,
    cc




  },
  head: {
    title: 'non-custodial',
    meta: [
      {
        hid: "2",
        name: "description",
        content: "Decentralized websites"
      }
    ]
  }

}
</script>

<style>
.display-3 {
  text-align: center;
  text-shadow: 2px 2px #42b983;
  -webkit-transform-style: preserve-3d;
  transform-style: preserve-3d;
}

.display-3:hover {
  -webkit-transform: rotateX(-169deg) rotateY(174deg) rotateZ(0deg)
    rotateX(-180deg) rotateY(0deg) rotateZ(0deg) rotateX(0deg) rotateY(180deg)
    rotateZ(0deg);
  transform: rotateX(-169deg) rotateY(174deg) rotateZ(0deg) rotateX(-180deg)
    rotateY(0deg) rotateZ(0deg) rotateX(0deg) rotateY(180deg) rotateZ(0deg);
}

h2 {
  text-align: center;
}
@media only screen and (max-width: 360px) {
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
}
.logo {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.about {
  background-color: #3c1d40;
  border: 2px solid;
}
</style>