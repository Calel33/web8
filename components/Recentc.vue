<template>
  <div class="cara">
    <b-container>
      <b-row>
        <b-col>
          <b-carousel
            id="carousel-fade"
            style="text-shadow: 0px 0px 2px #000"
            fade
            indicators
            img-width="1100"
            img-height="500"
            text-variant="dark"
          >
            <b-carousel-slide
              caption="Unstoppabledomains"
              img-src="../static/ud main.jpg"
            ></b-carousel-slide>
            <b-carousel-slide
              caption="Ethereum Name Service"
              img-src="../static/ens main3.jpg"
            ></b-carousel-slide>
            <b-carousel-slide
              class="etrade"
              caption="Efin dex"
              img-src="../static/Trading Screen.png"
            ></b-carousel-slide>
          </b-carousel>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "Recentc"
};
</script>

<style>
.carousel-item {
  border: 4px solid #42b983;
}
</style>
