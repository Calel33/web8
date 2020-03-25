<template>
  <div id="app">

    <Navbar />
    <pricec />
    <newsc />
    <br>
    <div>
      <adc1 class="flex-container" />
    </div>
    <br />

    <br>
    <br>
    <div class="top">
      <h1 class="display-4">

        Anansiweb8
      </h1>

      <img
        style="width:50%;"
        class="logo"
        alt="anansiweb logo"
        src="../static/anansilogoabout.png"
      />
    </div>

    <br />
    <welcomec />
    <br />
    <h1 class="display-4">

      Recently Added
    </h1>
    <recentc />

    <br />

    <cc />
  </div>

</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
import pricec from "../components/Pricec";
import welcomec from "../components/Welcomec";
import recentc from "../components/Recentc";
import adc1 from "../components/adc1";
import newsc from "../components/Newsc";
export default {
  name: "Abouta",
  components: {
    Navbar,
    cc,
    pricec,
    welcomec,
    recentc,
    adc1,
    newsc,


  }
}
</script>

<style>
html,
body {
  width: 100%;
  height: 100%;
  margin: 0px;
  padding: 0px;
}
.display-4 {
  text-align: center;
  text-shadow: 2px 2px #344a5f;
  -webkit-transform-style: preserve-3d;
  transform-style: preserve-3d;
}

.display-4:hover {
  -webkit-transform: rotateX(-169deg) rotateY(174deg) rotateZ(0deg)
    rotateX(-180deg) rotateY(0deg) rotateZ(0deg) rotateX(0deg) rotateY(180deg)
    rotateZ(0deg);
  transform: rotateX(-169deg) rotateY(174deg) rotateZ(0deg) rotateX(-180deg)
    rotateY(0deg) rotateZ(0deg) rotateX(0deg) rotateY(180deg) rotateZ(0deg);
}

h2 {
  text-align: center;
}

/* Small devices (portrait tablets and large phones, 600px and up) */

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #app {
    width: 100%;
  }
}
.logo {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
#app {
  background-color: #42b983;
  border: 2px solid;
}
.footer {
  background-color: #344a5f;
}
.ad1 {
  float: inline-end;
}
.top {
  padding-right: 3%;
}
@media only screen and (min-width: 320px), (max-width: 360px) {
  .newsf {
    width: 100%;
  }
}
</style>