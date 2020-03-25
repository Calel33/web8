<template>
  <div
    id="widget_horizontal_container"
    class="price"
  >
    <div class="widget_horizontal_iframe_container">
      <iframe
        src="https://widget.coinlib.io/widget?type=horizontal_v2&theme=dark&pref_coin_id=1505&invert_hover=no"
        width="100%"
        height="100%"
        scrolling="auto"
        marginwidth="0"
        marginheight="0"
        frameborder="0"
        border="0"
        class="widget_horizontal_iframe"
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: "Pricec"
};
</script>

<style>
#widget_horizontal_container {
  width: 100%;
  height: 82px;
  background-color: #1d2330;
  overflow: hidden;
  box-sizing: border-box;
  border: 1px solid #282e3b;
  border-radius: 4px;
  text-align: right;
  line-height: 14px;
  block-size: 62px;
  font-size: 12px;
  box-sizing: content-box;
  font-feature-settings: normal;
  text-size-adjust: 100%;
  box-shadow: inset 0 -20px 0 0 #262b38;
  padding: 1px;
  padding: 0px;
  margin: 0px;
}
.widget_horizontal_iframe_container {
  height: 42px;
  width: calc(100% - 1px);
}
.widget_horizontal_iframe {
  border: 0;
  margin: 0;
  padding: 0;
}
.widget_horizontal_powered {
  color: #626b7f;
  font-weight: 400;
  font-size: 11px;
  box-sizing: content-box;
  margin: 3px 6px 3px 0px;
  font-family: Verdana, Tahoma, Arial, sans-serif;
  float: right !important;
}
.widget_horizontal_powered_link {
  font-weight: 500;
  color: #626b7f !important;
  text-decoration: none;
  font-size: 11px;
  display: inline-block;
  margin-right: 5px;
}

@media only screen and (max-width: 300px) {
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
.price {
  align-self: baseline;
  top: -54%;
  position: relative;
}
</style>
