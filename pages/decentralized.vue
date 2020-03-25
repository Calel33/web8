<template>
  <div class="decen">
    <Navbar />
    <pricec />
    <br />

    <br />
    <div class="d">

      <h1 class="display-4">Decentralized Solutions</h1>

      <br />

      <b-card-group deck>

        <b-card
          bg-variant="dark"
          text-variant="white"
          title="Unstoppable Domains"
        >
          <b-card-text>
            Blockchain Domains #.CRYPTO #.ZIL
          </b-card-text>
          <b-button
            href="/udoverview"
            variant="primary"
          >More Info</b-button>
          <b-button
            href="https://unstoppabledomains.com/r/e8542f2138624e1"
            variant="danger"
          >Visit</b-button>
        </b-card>

        <b-card
          bg-variant="dark"
          text-variant="white"
          title="Etherum Naming service"
        >
          <b-card-text>
            Blockchain Domains #.ETH
          </b-card-text>
          <b-button
            href="/ensoverview"
            variant="primary"
          >More Info</b-button>
          <b-button
            href="https://ens.domains/"
            variant="danger"
          >Visit</b-button>
        </b-card>

        <b-card
          bg-variant="dark"
          text-variant="light"
          title="Efin Dex"
        >
          <b-card-text>
            Your keys your funds! #dex #trade.
          </b-card-text>
          <b-button
            href="/efinoverview"
            variant="primary"
          >More Info</b-button>
          <b-button
            href="https://efin.com/?rc=EFIN-B9LMP5X"
            variant="danger"
          >Visit</b-button>
        </b-card>

      </b-card-group>

    </div>
    <br />
    <cc />
  </div>
</template>

<script>
import Pricec from "../components/Pricec";
import Navbar from "../components/Navbar";
import cc from "../components/cc";

export default {
  name: "decentralized",
  components: {
    Navbar,
    Pricec,
    cc
  },
  head: {
    title: 'Solutions',
    meta: [
      {
        hid: "2",
        name: "solutions",
        content: "Decentralized/privacy"
      }
    ]
  }
};
</script>

<style>
h1.display-3 {
  text-align: center;

  text-shadow: 2px 2px #344a5f;
}

.decen {
  background-color: #42b983;
  border: 2px solid;
}

@media only screen and (min-width: 320px), (max-width: 360px) {
  .frame {
    overflow: hidden;
    width: 130%;
    display: flex;
  }
  .container {
    width: 100%;
  }
  .card-body {
    width: 100%;
  }
  h1.display-4 {
    width: 10%;
    white-space: pre-wrap;
  }
}
.card-body {
  box-shadow: 5px 10px #344a5f;
}
.card-body:hover {
  background-color: #344a5f;
}
.dbutton {
  justify-content: center;
  display: flex;
}

.display-4 {
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
</style>
