<template>
  <div class="ens">
    <title>Unstoppable Domains</title>

    <Navbar />
    <pricec />

    <br />

    <h2
      class="display-4"
      id="title"
    >

      ENS

    </h2>

    <br>
    <b-container>
      <h1 class="display-4">Overview</h1>
      <enscara />
    </b-container>
    <br>

    <section class="list1">
      <h1 class="display-4">Features</h1>

      <ul id="example-1">
        <li
          class="display-4"
          v-for="item in items"
          :key="item.message"
        >
          {{ item.message }}
        </li>
      </ul>

    </section>
    <br>

    <section class="integrations">
      <h1 class="display-4">Integrations</h1>

      <b-container>
        <b-row>

          <b-col>

            <li>
              <h3>Opera Touch</h3>
            </li>
            <a href="https://www.opera.com/mobile/touch">
              <img
                alt="Opera Touch"
                src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxAODg8QDxAQEBAQEBAQDw8PEg8WDxAQFRIWFhcRFRUYHSggGBolGxUXITEhJSkrLjAuFx8zODMsNygtLisBCgoKDg0OFxAQFy0lHyUtLS0tKy0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLf/AABEIAOEA4QMBEQACEQEDEQH/xAAcAAEAAgIDAQAAAAAAAAAAAAAAAQcFBgIECAP/xABCEAACAgADBAYGBwYEBwAAAAAAAQIDBBESBQYhMQcTQVFhcSJygZGhsRRCQ1JiksEjMlOCstEzY3PhJCVEZIPC8P/EABsBAQACAwEBAAAAAAAAAAAAAAABBQIDBAYH/8QAKxEBAAICAQMEAQMEAwAAAAAAAAECAxESBAUxEyFBUSIyYXEVQlKBM5Gh/9oADAMBAAIRAxEAPwC8QAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACGwiZiHCV8FzlFebRlFLT8MPVp/lCI4iD5Ti/JoTS0fB6tP8AKH0TMdM4tE+EhIAAAAAAAAAAAAAAAAAAAAABAAD5YjEwqi5WSjCPfJ5GVaWtOohhe9aRu0tc2hvnVDNUxdj+8+Ef7nfi7de36vZXZu5Ur+n3YHFb04qzlNVrugln72d9O346+Y2rsnX5r/OmMuxtln79k5etKT+B0xgpHiIctsmSfNpfDUu4y4R9MJ5fZqXchxj6I5PrVipw/cnOPqykvkzGcNZ8wyjJkjxaWSwu82Kr+01rusSfx5nPfocVvjTqx9bnp87Z3Ab6QeSvg4/ihxj7uZw5e22j3pKww9zifa8NkweNrujqqnGa8HxXmivyYrUnVo0sseWuSN1l2DBsSAAAAAAAAAAAAAAAAAAIbEDVtvb3wpbroyssXBy+zi/1ZY9N2+2T8r+0ODqOsivtTy0jG7Rtvlqtm5vx5LyXJF1j6emONVhU5L2yTuZdfWbtNXA1jicINY0cHC3ERgtU5KKXbJpIifZlXFNp1EMFjd76K81WpXP8PCP5n+hpnNWHbj7be36vZh799MS/3K6YLx1TfvzXyNc5pl117ZSPMuq97Mb/ABILyrh+ph61m3+nYfpzq3vxi5uqXnXl8mjKM1vlFu24viGW2Zv9ZVNSlXKEl9eifzjL+5FrVvGrw1f0+1J3Sy0t0+kvD4rKu6cYzfBTy0/mi+XmuBW5+ij9WOf9N1MuSv45I/236E00mmmnxTXJorZiYdUTtyCQAAAAAAAAAAAAAADhZNRTlJpJLNt8ku8RXc+yJlXW9G90r3KrDtxq5SmuErPLuiX/AEXborq2Tyreo6ibe1Wray24uHiaxxOJrHE4mscTi6NuNtsm6cFRZir+1VRbhD1pcjlzdRTH7TLtwdFz97e0OUejDbOMeu90VZ8o3XNuP8tcZJe8rMnXUmfO1njx48caiE39DO0orONuDsf3VZbF/GGRrjrcf1Lbyhq+2tztoYHN4nC2RivtI5Tq/NFvL25G6malvEstxLB6DcnSdANGgGhR7e3vCJrEw3zcXpHv2fKNWJ1X4VtJp8bal96HevA5s/Txk948sPS14X1s/HVYmqF1M42VWRUoTi+DRU2rMTqWOnZIQAAAAAAAAAAAABDECtd995uvlLD0v9jF5WSX2kl2eqj0Pbug4x6l49/hw58nL8YajqLjTk4GoaTxNQ0cUaho4tn3b3PnjUrL3KrDvko8LLl4P6sfHmyl67uHH8Mfl2YMER+VlkbN2bTha1Vh64VQXKMEl7+9lFa82ncy7HbyMQAiUU000mnwafJoCut9ui+jFKV2CUaMRxbguFNr7mvqvxR2Yerms6t4bK3+1J4vBTpsnVbBwsrk4zhJZOMu4ta2i0bhviPl8tBJo0A0aAabn0b74y2Xd1djbwlsv2kf4Un9rHu8UcnU4IvG48sL029A1WxnGMotSjJJxkuTT5NFRMTE6c7mAAAAAAAAAAAIIGodIO8H0apYeqWVty9JrnCvln5vkvaW3bOk9W/O3iGrLbUahV+o9Px17OPiaidHE1jRxNQ0ni23cXdz6XPr7lnRW8oxfK2a7PVRTdz63049OnmW3Fi3O5Wklly5Hm5l1gEgAAADR+krcyO0KXfTFLF1R9Fr7aC49XLx7mdXTZ5pOp8NmO+p1KiZVtNpppptNPmmuaZcxr4dcQjQNGjQDRoHg0tnoe3pb/5dfLknLCyf3VxlV7Oa8M+4reswa/OHPlx/K1SuaEgAAAAAAAAAHxxeIjVXOybyjCLlJ+CRlSs3tFYFF7Y2lLFYiy+fOcm0vuxXCMV5I9t0uCMOKKQ5re8unqOjTHiZjSdGoaNO5snAyxV9dMOdkks+5dsvdmc/UZow47Xkiu5XjgMHDD1QqrWUYRUUv1PFZMk3tNp8y6YjUOyYJAAAAAAhgUr0sbuLDYpYmtZVYlvUlyjclm/LNcfeW3RZeUcZdeC2400TQd7o0aBo0aAafXCXTptrtremyucZwkuySeaMb05RpE13Gno/d7ascbhacRD7SKcl92f1o+88/lpNLzWVfevGdMkYMQAAAAAAAABpPSjtTqsLCiLylfL0v9OPF/HJFv2fB6mWb/SLKr1Hq9NejUNGjUNGjUNGlh9FGzc+uxUlyfU1+eWc2vfFe8853vP71xR/LOsLGKBkkAAAAAAADB76bHWOwF9KXp6ddXhbDjH35ZeTZu6fJ6eSJbMVuNol57Uf/megj7WejSSaNINGkg0s/ob2rk78JJ/51afukvk/aVfX4/FnH1NP7lola5AAAAAAAACGBTfSVj+t2jOCfo0QhWvWa1P5r3HruzYuGDf2TDVcy20jRmDRmDQ5CTS9NzcD9H2fhoZZSdanP15+k/n8Dw3XZPU6i8/ulmzkAAAAAAAACGB5/wB7tn/R9oYqtLKPWOcfVn6X6s9D01uWOJW2Gd1iWH0m5s0aCTRpBpmtzMZ9G2jhbOSdirl6tno/Np+w5+ppyxS1Zq7pK/jz6qSAAAAAAAAA89bZxPXYrE2ffvtkvLW8vhke96WnHDSP2hlp0zo0aMwaAafXB1dZbXD79kIfmkl+przzxx2n9jT0TVDTGK7kl7kfP7TuWLmQAAAAAAAAACoelfC6cdCf8Sle+Ly/Uue3zukwsukndWlaSwdmk6QaNINI4x9Jc4+kvNcURMbjSJj2ejMHcrKq5rlOEZL2xTPMXjVphSWjUzD7kMQAAAAAAHC6WUZPuTfwJrG5iEx5eb08+Pfx959CxxqkQzDMCQI0Mlu1DVjsIv8APh8Hn+hyddOsF/4kl6BPCNYAAAAAAAAAAVn0uw/aYV/hmvii17b4sseh8Sr7SWqw0aQaNINDiNImF8brT1bPwbfbhqf6EeazxrJb+VHmjV5ZU1NYAAAAAADhfHOEl3xa+BlWdWiUx5eborgj6DjndYZpMwAEwMnuzLLH4R/58Pi8jj66N9Pf+CXoA8I1gAAAAAAAAABW/Sy854Vfhm/ii27ZHtZZdBHtZoGktVjo0g0aQaRpBMLz3Vjp2fg1/wBvT/QjzOed5LKHN/ySypqagAAAAAAADzttTD9Vib6+XV3Ww9im0j6B014vhpMfUNjqm8CAA7Gz7urvpn9y2uXsUkzVnryxXj9pJeiYSzSfekz5/PtLW5EAAAAAAAABAFXdKF2rF1w+5V/U/wDYuu211SZW3QV/CZadkWTv0ZA0ZA0hxz5c3wXmJnSJ9oX5gKerpqh9yuEfdFI8red2mXnbzu0y7BixAAAAAAAAKT6RsF1O0rnlwuULV5tZP4x+J7Hs+Xn08R9ezOGsFskIAkGiJjcaF+bp476RgMNbzbqipevH0ZfFM8F1mP0896/uwllzmQAAAAAAAAQwKY3uxfX4/ESTzSloXlHh88z0fR044YX/AE1OOKIYfI6nQZAMgMlu5g+vxuHr5p2RlL1Y+k/kc/U344rS0dRbjjmV2o81Lz6QAAAAAAADAr/pa2XroqxMVxqlon6kv90i77Jn4ZJpPyyqqw9YyAAACzuiPamdd+Fk+MJddX6sslJeySz/AJjy3fMGr1yx4n2Y2hYpQsQAAAAAAADHbwbQWFwt1z5xj6K75vhFe9o24MfO8VbcGPneIUo83xfFvi33t9p6aNRD0URqNIyJ3CdGQ2aMhEwabv0ZbO1W24hrhBdXDzfF/oVXccvtFIVncMntFYWKVCqSAAAAAAAAA6u08FHE0WUz/dsg4vwz7TZhyTjvF4+CHn7aODnh7rKbFlOuTi/ZyftXH2nvMGauWkXj5bYdY2gSAGS3d2s8Fiqr1yi8prvg+El7jk63p46jFNUSv3DYiNsI2QalGcVKLXJpnhb1mszWWt9SAAAAAACAK86RNq9ZZHDQeca3qsy7Z5cF7F8yy6KnH8pW/b8GvzlpugsOa01s0DmaNA9Q0mFTk1FLNyaSS5tt5JETk1EyxmYrEzK4t3tmrCYaur6yWc33zfFlHmyTe8y85nyepeZZM1NIAAAAAAAAAgCvOlPd3rILG1RznXFRvS+tWuU/NfLyLzs/W8J9K3ifDKsqtzPT7bNJzJ2jRmNp0ZjyaWF0Z71KtrBXyyhJ/wDDzfKMn9m349nuPPd26He81I/ljaFpHnGtIAAAAgDDbzbajhKuGTtmmq4/+z8EbMVOUurpemnNf9lW2Nyk5SecpNtt822WPLUREPQ1rqIiPDjoJ9Rl8mgczRoHM027cTYmuz6TYvRg2qk+2fbL2fM5uoze3GFX3DqNRwj/AG384lMkAAAAAAAAAAAcbIKSaaTTTTT5NPsETMTuBSu/u6rwFvW1JvDWS9F/wpP6j8O49Z23r/WrwtP5R/621nbU8y12y0ZjZozGw1ETqY1JpZ+42/qko4fGS9JZKu5/WXYp+PieZ7h27hPqY/B6XL9KxoTUkmmmnxTXJlK0zEx5cggAAYXbm8VWGTisp29kF2eMn2GUVdnT9HfLP7K8xuIsvslZbJylLt7EuxJdiN9bahf4sNcdeNXX0E82w6sczRoHM1tk9g7Fli7dPFVxydk+5dy8WY2yOXq+ojDX91nYeiNcIwgkoxSSS7EjRM7ebvebTuX1IQAAAAAAAAAAAAB18dg67651WxU65pxlGXJoypktjtFq+UxKld9NzbdnSdkNVmFb9Gf1q/wz/ueo6LuNc3429rNtZ21TUWUWbNGocjRqHI0aiJmJjUp8TuG07ub534XKErHp7G+Mf5ov5oo+t7bFvyxf9OqtseT2yR/tvuD33nKKbrrsT+tCbSfwZQ3rak6tGmz+mUvG6XfezfR5ejh1n42f2ia+ZHaZ+bf+MVjt48VcmtSri+ytZfF8SebrxdvxU99blh3Ec3bFdR7I0Dmk0DmaToHOR3ti7Jni7NMeEIv9pZ2R8PGRnqflxdT1dMUe3lYuz8FDD1qutZRXvb7W+9kPPZctsluVnaDWAAAAAAAAAAAAAAAcLqozi4ySlGSylFrNNdzRMTMTuBV+9/Rm/Su2d4uWFk0l/wCOT5eTLjpe5zH45P8Atvpk+1Y4mqdM5V2wlXOLylCaakvYy3pmi0biW+Pfw+XWGXM4nWDmnidYPUOLsYTaFlLzrm4967H5o0ZcOPL7WhspktTxLO4Te3krq8/xVvJ+5lPm7Tv/AI5d1OumP1QylO8eElzscPCcJL4rNFfk7fnr8bdNerxy7C2vhX/1FX5kjTPS5/8ACWz18f24Wbcwked8H6uqXyRlXos9vNUT1GOPl0rd6KW1GmFls3wilHLN9yXN+46qdryebzqGi/XUjw2rd/dTGYvKzHf8LS+Kw8H+2mvxy+ovDn5E29HF7U95+1Zn7he3tCw8HhK6IRrqgoQisoxiskjmtaZVs2mfeXYIQAAAAAAAAAAAAAAAAAEAYvbe72Fx0dOJpjPhkp8px8pLibMea9J/GWVbzHhW+3eiKxZywN6kuyq/NPyU1+qLDH3Gf7odFc8f3NF2puttHCZ9dhLtK+vXHrIeecM8vbkdderpbxLfF6T4lgnes8m8n2p8/cbPWbOKetHqnE60eqnih4hd6HrI4svsvd/HYtrqMJfNPlNwca/zSyRhbqq18ywtatfMt42H0SYizKWMujTHtrq9Kftk+COXJ3H4q0Xzx/asnd/dTB7PX7Cla+22fpWP+Z8vYV+XqL5P1S57ZJt5Zs0MEkgAAAAAAAAAAAAAAAAAAAAABAHUxey8Pf8A41FNv+pXCXzRMWtHiWUWmPli7NyNly57Pwv8tUI/JGz1r/bL1b/aIbj7Kjy2fhfbVF/Mj1r/AGerf7ZLB7GwtH+DhsPVl/Dqrj8kYze0+ZYze0+Zd7IxYgEgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAf/9k="
              /></a>
          </b-col>
          <b-col>
            <h3>
              <li>Atomic</li>
            </h3>

            <a href="https://atomicwallet.io/">
              <img
                alt="Atomic"
                src="https://unstoppabledomains.com/_next/static/images/atomic-logo-387374d0f0e665c037cdea5a7436c2b3.png.webp"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>MYCrypto</li>
            </h3>
            <a href="https://opensea.io/">
              <img
                alt="MyCrypto"
                src="https://ens.domains/static/myCrypto.0d0e7058.png"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>OpenSea</li>
            </h3>
            <a href="https://mycrypto.com/">
              <img
                alt="Opensea"
                src="https://ens.domains/static/opensea.d885f10a.png"
              /></a>
          </b-col>
        </b-row>
      </b-container>

      <b-container>
        <b-row>

          <b-col>
            <h3>
              <li>Coinonmi</li>
            </h3>
            <a href="https://www.coinomi.com/en/">
              <img
                alt="Coinomi"
                src="https://ens.domains/static/coinomi.fe6a7f77.png"
              /></a>
          </b-col>
          <b-col>
            <h3>
              <li>DefSwamp</li>
            </h3>
            <a href="https://defswap.eth.link/">
              <img
                alt="DefSwamp"
                src="https://ens.domains/static/defswap.f4031e57.png"
              /></a>
          </b-col>

          <b-col>

            <h3>
              <li>Etherscan</li>
            </h3>
            <a href="https://etherscan.io/">
              <img
                alt="EtherScan"
                src="https://ens.domains/static/etherscan.4795fc5c.png"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>EthSimple</li>
            </h3>
            <a href="https://ethsimple.com/">
              <img
                alt="ETHsimple"
                src="https://ens.domains/static/ethsimple.5e3d4ed0.jpg"
              /></a>
          </b-col>
        </b-row>
      </b-container>
      <b-container>
        <b-row>
          <b-col>

            <h3>
              <li>TrustWallet</li>
            </h3>
            <a href="https://trustwallet.com/">
              <img
                alt="Trustwallet"
                src="data:image/png;base64,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"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>imToken</li>
            </h3>
            <a href="https://token.im/">
              <img
                alt="Imtoken"
                src="https://ens.domains/static/imToken.2f7546bf.png"
              /></a>
          </b-col>
          <b-col>
            <h3>
              <li>MetaMask</li>
            </h3>
            <a href="https://ens.domains/static/metamaskmobile.e382144e.png">
              <img
                alt="Metamask"
                src="https://ens.domains/static/metamask.e382144e.png"
              /></a>
          </b-col>
          <b-col>
            <h3>
              <li>MailChain</li>
            </h3>
            <a href="https://mailchain.xyz/">
              <img
                alt="MailChain"
                src="data:image/png;base64,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"
              /></a>
          </b-col>
        </b-row>
      </b-container>

    </section>

    <br>
    <section class="end">
      <hr>
      <h1 class="display-4">Get .ETH!</h1>
      <ul>
        <li>
          <a href="https://ens.domains/">
            <b-button variant="danger">Visit ENS</b-button>
          </a>
        </li>

        <a href="https://medium.com/the-ethereum-name-service">
          <li>
            <font-awesome-icon
              :icon="faMedium"
              size="lg"
            />
          </li>
        </a>
        <a href="https://twitter.com/ensdomains">
          <li>
            <font-awesome-icon
              :icon="faTwitter"
              size="lg"
            />
          </li>
        </a>
        <a href="https://github.com/ensdomains">
          <li>
            <font-awesome-icon
              :icon="faGithub"
              size="lg"
            />
          </li>
        </a>

      </ul>

    </section>

    <br />

    <cc />
  </div>

</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
import pricec from "../components/Pricec";
import enscara from "../components/enscara";

import { faGithub } from "@fortawesome/free-brands-svg-icons";
import { faMedium } from "@fortawesome/free-brands-svg-icons";
import { faTwitter } from "@fortawesome/free-brands-svg-icons";

export default {
  name: "ud",
  components: {
    Navbar,
    cc,
    pricec,
    enscara




  },
  data () {
    return {
      faGithub, faMedium, faTwitter,

      items: [

        { message: "Premium domains" },
        { message: "Tor intergration" },

        { message: "Subdomain" },
        { message: "Self Custody" },
        { message: "Accept ETH via domain " },
        { message: "Smart contract" },

        { message: "Readble human addresses" },
        { message: "Build uncensorable website" },
        { message: "renewal fees start @ 0.033eth per year" },
        { message: "Robust ecosystem" },
        { message: ".ETH variant (Ethereum blockchain)" },
      ],

    };
  },
  head: {
    title: 'ENS Overview',
    meta: [
      {
        hid: "2",
        name: "description",
        content: "Ens,.eth"
      }
    ]
  }
};


</script>

<style>
html,
body {
  width: 100%;
  height: 100%;
  margin: 0px;
  padding: 0px;
}
.ens {
  background-color: #344a5f;
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

h1 {
  text-align: center;
}

li {
  justify-content: center;
  display: flex;
}
img {
  height: 101px;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
