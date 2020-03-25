<template>
  <div class="Denybw">

    <section class="top">

      <navbar />

    </section>

    <section>

      <h1 class="display-4">DenyB DomainWall</h1>

    </section>

    <br>

    <template class="dm">
      <b-container-deck column>
        <b-row>
          <b-col>

            <div class="flip-card">
              <div class="flip-card-inner">
                <div class="flip-card-front">
                  <img
                    src="../static/cs.zil.png"
                    alt="
                    Avatar"
                    style="width:300px;height:300px;"
                  >
                </div>
                <div class="flip-card-back">

                  <h2>CITYSEARCH.ZIL</h2>
                  <h1>price: {{price1}}
                    <font-awesome-icon
                      :icon="faEthereum"
                      size="md"
                    />
                  </h1>

                  <br>

                  <b-button href="/DomainVision">View Vision</b-button>
                  <br>

                  <a
                    href="mailto:denmatix@gmail.com"
                    to="mailto:denmatix@gmail.com"
                    target="_blank"
                    rel="noopener noreferrer"
                  >

                    <font-awesome-icon
                      class="bottom"
                      :icon="faEnvelope"
                      size="lg"
                    />

                  </a>

                </div>
              </div>
            </div>

          </b-col>

          <b-col>

            <div class="flip-card">
              <div class="flip-card-inner">
                <div class="flip-card-front">
                  <img
                    src="https://storage.opensea.io/files/6d1e82aad02bd2d3b073518ab1da80ee.svg"
                    alt="Avatar"
                    style="width:300px;height:300px;"
                  >
                </div>
                <div class="flip-card-back">
                  <h2>THINKMEDIA<wbr>.CRYPTO<wbr></h2>
                  <h1>price: {{price2}}
                    <font-awesome-icon
                      :icon="faEthereum"
                      size="md"
                    />
                  </h1>

                  <br>

                  <b-button href="/Domainvision">View Vision</b-button>
                  <br>
                  <b-button
                    style="margin-top:3%;"
                    href="https://opensea.io/assets/0xd1e5b0ff1287aa9f9a268759062e4ab08b9dacbe/55645345370603154057410265935222738629937863619088763738044448677604929493613"
                  >Buy On Opensea</b-button>

                  <a
                    href="mailto:denmatix@gmail.com"
                    to="mailto:denmatix@gmail.com"
                    target="_blank"
                    rel="noopener noreferrer"
                  >

                    <font-awesome-icon
                      class="bottom"
                      :icon="faEnvelope"
                      size="lg"
                    />

                  </a>

                </div>
              </div>
            </div>

          </b-col>

          <b-col>

            <div class="flip-card">
              <div class="flip-card-inner">
                <div class="flip-card-front">
                  <img
                    src="../static/superbets.png"
                    alt="Avatar"
                    style="width:300px;height:300px;"
                  >
                </div>
                <div class="flip-card-back">
                  <h2>SUPERBETS.ZIL</h2>
                  <h1>price: {{price3}}
                    <font-awesome-icon
                      :icon="faEthereum"
                      size="md"
                    />
                  </h1>

                  <br>

                  <b-button href="/Domainvision">View Vision</b-button>
                  <br>

                  <a
                    href="mailto:denmatix@gmail.com"
                    to="mailto:denmatix@gmail.com"
                    target="_blank"
                    rel="noopener noreferrer"
                  >

                    <font-awesome-icon
                      class="bottom"
                      :icon="faEnvelope"
                      size="lg"
                    />

                  </a>

                </div>
              </div>
            </div>

          </b-col>
        </b-row>
      </b-container-deck>
    </template>
    <br>
    <br>
    <cc />
  </div>

</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
import { faEnvelope } from "@fortawesome/free-solid-svg-icons";

import { faEthereum } from "@fortawesome/free-brands-svg-icons";

export default {
  name: "domianwall",
  components: {
    Navbar,
    cc




  },


  data () {
    return {
      price1: 3,
      price2: 10,
      price3: 8,





      faEnvelope,

      faEthereum

    }
  },
  head: {
    title: 'DenyBWall',
    meta: [
      {
        hid: "2",
        name: "Domain wall",
        content: "Domain wall, "

      }
    ]
  }
}
</script>

<style scoped>
* {
  box-sizing: border-box;
}

.display-4 {
  text-align: center;
  text-shadow: 2px 2px #42b983;
  margin-bottom: 5%;
  margin-top: 5%;
}

h2 {
  text-align: center;
}

.flip-card {
  background-color: transparent;
  width: 300px;
  height: 300px;
  perspective: 1000px;
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
  background-color: #344a5f;
  color: darkgray;
  transform: rotateY(180deg);
}

.row {
  margin-right: 10px;
}

.bottom {
  position: absolute;
  bottom: 0;
  left: 0;
}

.bottom2 {
  position: absolute;
  bottom: 0;
  left: 2em;
}

.bottom3 {
  position: absolute;
  bottom: 0;
  left: 4em;
}

.flip-card {
  margin-bottom: 15%;
  margin-left: 8%;
}
.Denybw {
  background-color: #1c1c1c;
}
</style>