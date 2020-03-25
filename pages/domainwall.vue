<template>
  <div class="about">

    <Navbar />
    <br />
    <h1 class="display-3">

      Domain Wall
    </h1>
    <br>
    <section>
      <template>
        <b-row>
          <b-col>

            <div class="flip-card">
              <div class="flip-card-inner">
                <div class="flip-card-front">
                  <img
                    src="https://images.unsplash.com/photo-1526374965328-7f61d4dc18c5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80"
                    alt="Avatar"
                    style="width:300px;height:300px;"
                  >
                </div>
                <div class="flip-card-back">
                  <h1>TechGuy Domian Wall</h1>

                  <b-button
                    style="margin-top:7%;"
                    href="/Techguywall"
                  >View Wall</b-button>
                </div>
              </div>
            </div>
          </b-col>
          <b-col>

            <div class="flip-card">
              <div class="flip-card-inner">
                <div class="flip-card-front">
                  <img
                    src="https://cdn.pixabay.com/photo/2016/03/09/15/10/explosion-1246507_960_720.png"
                    alt="Avatar"
                    style="width:300px;height:300px;"
                  >
                </div>
                <div class="flip-card-back">
                  <h1>DenyB Domain Wall</h1>
                  <b-button
                    style="margin-top:7%;"
                    href="/Denybwall"
                  >View Wall</b-button>
                </div>
              </div>
            </div>

          </b-col>

        </b-row>
      </template>

    </section>
    <br />
    <br>
    <cc />
  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
import { faTwitter } from "@fortawesome/free-brands-svg-icons";
export default {
  name: "domianwall",
  components: {
    Navbar,
    cc




  },

  data () {
    return {
      faTwitter,

    }
  },
  head: {
    title: 'Domain Wall',
    meta: [
      {
        hid: "",
        name: "Domain Wall",
        content: "Domain .Crypto .ETH .ZIL"
      }
    ]
  }
}

</script>

<style scoped>
.display-3 {
  text-align: center;
  text-shadow: 2px 2px #42b983;
  margin-bottom: 5%;
  margin-top: 2%;
}
h2 {
  text-align: center;
}
@media only screen and (min-width: 320px), (max-width: 360px) {
  card-img {
    width: 500px;
  }
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

.about {
  background-color: #071a52;
  border: 2px solid;
}

.display-3 {
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

.flip-card {
  background-color: transparent;
  width: 300px;
  height: 300px;
  perspective: 1000px;
  margin-bottom: 15%;
  margin-left: 8%;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

.flip-card-front,
.flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
}

.flip-card-front {
  background-color: #bbb;
  color: black;
}

.flip-card-back {
  background-color: #086972;
  color: #17b978;
  transform: rotateY(180deg);
}

/* Float four columns side by side */

/* Remove extra left and right margins, due to padding in columns */
.row {
  margin-right: 10px;
}

/* Clear floats after the columns */

/* Responsive columns - one column layout (vertical) on small screens */
</style>