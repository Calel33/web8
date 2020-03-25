<template>
  <div class="enscara">
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
              caption=""
              img-src="../static/ens main3.jpg"
            ></b-carousel-slide>
            <b-carousel-slide
              caption=""
              img-src="../static/ensmain.jpg"
            ></b-carousel-slide>
            <b-carousel-slide
              caption=""
              img-src="../static/ens main2.jpg"
            ></b-carousel-slide>

          </b-carousel>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "enscara"
};
</script>

<style>
</style>
