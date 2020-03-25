<template>
  <div class="Newsc">
    <iframe
      class="newsf"
      width="50%"
      scrolling="yes"
      allowtransparency="true"
      frameborder="0"
      src="https://cryptopanic.com/widgets/news/?bg_color=202328&amp;font_family=sans&amp;header_bg_color=30343B&amp;header_text_color=FFFFFF&amp;link_color=0091C2&amp;news_feed=recent&amp;posts_limit=6&amp;text_color=33333&amp;title=Latest%20News"
      height="100px"
    ></iframe>
  </div>
</template>

<script>
export default {
  name: "Newsc"
};
</script>

<style scope >
.news {
  position: relative;
  right: -5%;
  border: 2px solid;
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
iframe {
  border: 2px solid;
}
</style>
