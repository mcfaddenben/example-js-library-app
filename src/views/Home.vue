<template>
  <div class="carousel">
    <h1>Best SC fighters</h1>
    <VueSlickCarousel v-bind="settings">
      <img
        src="https://star-hangar.com/media/catalog/product/cache/a374beeb149e9f7dce9709647a4d8d34/1/1/1199px-sabre_-_firing_x2_-_front.png"
        alt="Aegis Sabre"
      />
      <img src="https://i.ebayimg.com/images/g/w1kAAOSwLqpgtZDY/s-l300.jpg" alt="Esperia Talon" />
      <img
        src="https://cdnb.artstation.com/p/assets/images/images/025/061/055/large/jeremiah-lee-arrow-concept-v3-bottom.jpg?1584468627"
        alt="Anvil Arrow"
      />
      <img src="https://media.robertsspaceindustries.com/9cwz2utclixvt/source.jpg" alt="Aegis Gladius" />
      <img src="https://media.robertsspaceindustries.com/6ewzke6o3llh6/source.jpg" alt="Anvil F7CM Super Hornet" />
    </VueSlickCarousel>
  </div>
</template>
<style>
.carousel {
  max-width: 600px;
  margin-left: 25%;
}
</style>
<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  data: function () {
    return {
      settings: {
        arrow: true,
        dots: false,
        fade: true,
        infinite: true,
        speed: 700,
        slidesToShow: 3,
        slidesToScroll: 1,
      },
    };
  },
  components: { VueSlickCarousel },
};
</script>
