<template>
  <div class="dbutton">
    <b-button v-b-modal.modal-1><em>anansiweb8.zil</em>
      <font-awesome-icon
        :icon="faBitcoin"
        size="lg"
      />
      <font-awesome-icon
        :icon="faEthereum"
        size="lg"
      />
    </b-button>

    <b-modal
      id="modal-1"
      title="anansiweb8.zil"
    >
      <p class="my-4">
        You can donate multiple cryptos to <em>anansiweb8.zil</em> via imToken, Trustwallet, Atomic,
        Coinomi, more intergrations coming! Thank You!
      </p>
    </b-modal>

  </div>

</template>

<script>
import { faBitcoin } from "@fortawesome/free-brands-svg-icons";
import { faEthereum } from "@fortawesome/free-brands-svg-icons";
export default {
  name: "dbutton",

  data () {
    return {
      faBitcoin,
      faEthereum
    };
  }
};
</script>

<style>
.dbutton {
  justify-content: space-around;
  display: flex;
}
</style>
