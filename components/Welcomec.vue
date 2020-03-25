<template>
  <div>

    <div>
      <b-jumbotron
        class="h3"
        style="background-color:#086972"
      >
        <template
          v-slot:header
          style="overflow-wrap: break-word"
        > Decentralized and Privacy Solutions</template>

        <template v-slot:lead>
          Web3 is here at its early stages the dream of a decentralized, secure,
          and private internet is coming to realilty.
        </template>

        <hr class="my-4" />

        <p>
          Find decentralized websites and privacy/decentralized solutions, blocksites,and things blockchain,
        </p>

        <b-button
          variant="primary"
          href="/decentralized"
        >Decentralized/Privacy</b-button>

        <b-button
          variant="primary"
          href="/blocksites"
        >blocksites</b-button>
      </b-jumbotron>

    </div>

  </div>
</template>

<script>
export default {
  name: "Welcomec"
};
</script>

<style>
.h1 {
  text-shadow: 2px 2px #344a5f;
}
.jumbotron {
  border: 2px solid;
  box-sizing: border-box;
}
@media only screen and (min-width: 320px), (max-width: 360px) {
  .display-3 {
    font-size: 150%;
  }
  .frame {
    overflow: hidden;
    width: 130%;
    display: flex;
  }
  .container {
    width: 100%;
  }
}
.frame {
  justify-content: center;
  display: flex;
}
</style>
