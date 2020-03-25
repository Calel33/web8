<template>
  <div class="vision">

    <Navbar />
    <br>
    <b-container>

      <b-row>

        <b-col>

          <h1>

            Anansiweb8.zil

          </h1>

        </b-col>

        <b-col>

          <h1 id="title2">

            Owner:Techguy

          </h1>

        </b-col>

      </b-row>
    </b-container>
    <section class="featureli">
      <h3 class="display-4">
        Features

      </h3>
      <ul>
        <h3>
          <li>Decentralized/Privacy Solution</li>
        </h3>
        <h3>
          <li>DomainWall</li>
        </h3>
        <h3>
          <li>DomainVision</li>
        </h3>
        <h3>
          <li>Tutorials (coming-soon)</li>
        </h3>
        <h3>
          <li>Blocksites</li>
        </h3>
        <h3>
          <li>Non-custodial wallets</li>
        </h3>
        <h3>
          <li>Blockchain Art(coming-soon)</li>
        </h3>

      </ul>
    </section>
    <section class="propli">

      <h3 class="display-4">
        Properties

      </h3>
      <ul>

        <h3>
          <li>.Zil</li>
        </h3>
        <h3>
          <li>Domain length:10 letters</li>
        </h3>
        <h3>
          <li>Numbers:1</li>
        </h3>
        <h3>
          <li>Specialkey:0</li>
        </h3>
        <h3>
          <li>Badges(coming-soon)</li>
        </h3>

      </ul>
    </section>
    <section class="propli">

      <h3 class="display-4">
        Monetization

      </h3>
      <ul>

        <h3>
          <li>Ad Space</li>
        </h3>
        <h3>
          <li>Domain Listing </li>
        </h3>
        <h3>
          <li>Blocksites Api</li>
        </h3>
        <h3>
          <li>Partnerships</li>
        </h3>
        <h3>
          <li>Marketplace Fee's</li>
        </h3>

      </ul>
    </section>
    <section class="propli">

      <h3 class="display-4">
        Possibilities

      </h3>
      <ul>

        <h3>
          <li>Blocksite Api</li>
        </h3>
        <h3>
          <li>Integrate Web3 </li>
        </h3>
        <h3>
          <li>Decentralized Solutions Api</li>
        </h3>
        <h3>
          <li>Integrate Smart Contracts (Zil-ETH)</li>
        </h3>
        <h3>
          <li>Enable Marketplace For Decentralized Things </li>
        </h3>
        <h3>
          <li>Domain Business Builder NFT Game </li>
        </h3>

      </ul>
    </section>

    <br>
    <section class="Targetm">
      <br>
      <h2>Targetmarket:Crypto audience, people, and entites that are looking for decentralization,
        privacy solutions and things blockchain. </h2>
      <br>
      <h2>Relevance:As technology advance and more of your data is exposed understanding decentalization and privacy is key
        you have the right to protect your privacy. </h2>
    </section>
    <br>
    <section class="summary">
      <h2>Summary:Provide decentralized and privacy solutions, blocksites and decentralized things. </h2>
    </section>

    <br>

    <br>

    <cc />

  </div>
</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
export default {
  name: "domianwall",
  components: {
    Navbar,
    cc




  },
  head: {
    title: 'Anansiweb Vision',
    meta: [
      {
        hid: "2",
        name: "vision",
        content: "vision, ideas"
      }
    ]
  }


}
</script>

<style>
.vision {
  background-color: #42b983;
}

.display-4 {
  text-shadow: 2px 2px #344a5f;
  text-align: center;
  margin-bottom: 2%;
  margin-top: 5%;
}

h1 {
  border: 2px solid;
}
@media only screen and (min-width: 320px), (max-width: 766px) {
  h1 {
    margin-right: 10%;
  }
}
ul {
  display: table;
  margin: 0 auto;
}
</style>