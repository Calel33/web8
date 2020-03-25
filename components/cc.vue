<template>
  <div class="footer">
    <footer class="container py-5">
      <div class="row">
        <div class="col-12 col-md">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            class="d-block mb-2"
            role="img"
            viewBox="0 0 24 24"
            focusable="false"
          >
            <title>Anansiweb8</title>
            <circle
              cx="12"
              cy="12"
              r="10"
            ></circle>
            <path d="M14.31 8l5.74 9.94M9.69 8h11.48M7.38 12l5.74-9.94M9.69 16L3.95 6.06M14.31 16H2.83m13.79-4l-5.74 9.94"></path>
          </svg>
          <small class="d-block mb-3 text-muted">© 2019 anansiweb8.zil</small>
        </div>
        <div class="col-12 col-md">
          <h5>Anansiweb8</h5>
          <ul class="list-unstyled text-small">
            <li><a
                class="text-muted"
                href="/Aboutanansi"
              >About</a></li>
            <li><a
                class="text-muted"
                href="/ads"
              >Advertise</a></li>
            <li class="li1">
              <a
                class="text-muted"
                href="/blocksites"
              >Blocksites</a>
            </li>
            <li><a
                class="text-muted"
                href="/domainwall"
              >DomainWall</a></li>
            <li>
              <a
                class="text-muted"
                href="/decentralized"
              >Decentralized/Privacy</a>
            </li>

            <li><a
                class="text-muted"
                href="/Non-custodialwallet"
              >Non-Custodial Wallets</a></li>
          </ul>
          <h5>Donations</h5>
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
                <b>You can donate multiple cryptocurrencies to <em>anansiweb8.zil</em> via imToken, Trustwallet, Atomic,
                  Coinomi, more intergrations coming! Thank You!</b>
              </p>
            </b-modal>
          </div>

        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import { faBitcoin } from "@fortawesome/free-brands-svg-icons";
import { faEthereum } from "@fortawesome/free-brands-svg-icons";
export default {
  name: "cc",
  data () {
    return {
      faBitcoin,
      faEthereum
    };
  }
};


</script>

<style >
.dbutton {
  justify-content: center;
  display: flex;
}

.footer {
  position: static;
  left: 0;
  bottom: 0;
  width: 100%;
  text-align: center;
  background-color: #344a5f;
  border: 2px solid;
}
</style>
