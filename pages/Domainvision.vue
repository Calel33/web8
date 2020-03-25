<template>
  <div class="vision">

    <Navbar />
    <br />
    <h1 class="display-4">

      Why have the domain<wbr> without the vision?<wbr>
    </h1>
    <br>
    <template>
      <b-row>
        <b-col>

          <div class="flip-card">
            <div class="flip-card-inner">
              <div class="flip-card-front">
                <img
                  src="../static/anansilogoabout.png"
                  alt="Avatar"
                  style="width:300px;height:300px;"
                >
              </div>
              <div class="flip-card-back">
                <h1>ANANSIWEB8<wbr>.ZIL<wbr></h1>

                <b-button
                  style="margin-top:7%;"
                  href="/anansiwebvision"
                >View Vision</b-button>
              </div>
            </div>
          </div>
        </b-col>
      </b-row>

    </template>
    <cc />

  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
;
export default {
  name: "domianwall",
  components: {
    Navbar,
    cc




  },
  head: {
    title: 'Domain Vision',
    meta: [
      {
        hid: "2",
        name: "Domain Vision",
        content: "Vision,Domain"
      }
    ]
  }


}
</script>

<style scoped>
html,
body {
  width: 100%;
  height: 100%;
  margin: 0px;
  padding: 0px;
}
.vision {
  background-color: #344a5f;
}
.display-4 {
  text-align: center;
  text-shadow: 2px 2px #42b983;
  margin-bottom: 5%;
  margin-top: 2%;
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
  background-color: #42b983;
  color: white;
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