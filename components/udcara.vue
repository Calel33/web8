<template>
  <div class="udcara">
    <b-container>
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
          img-src="../static/ud main.jpg"
        ></b-carousel-slide>
        <b-carousel-slide
          caption=""
          img-src="../static/ud pre.jpg"
        ></b-carousel-slide>
        <b-carousel-slide
          caption=""
          img-src="../static/ud addadress.jpg"
        ></b-carousel-slide>
        <b-carousel-slide
          caption=""
          img-src="../static/ud man.jpg"
        ></b-carousel-slide>
      </b-carousel>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "udcara"
};
</script>

<style>
.carousel {
  border: 4px solid;
  padding: 1px;
  box-shadow: 2px 2px;
}
</style>
