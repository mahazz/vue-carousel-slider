<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-sm">
          <div class="card slider">
            <carousel :per-page="1" :mouse-drag="false">
              <slide>
                <img src="@/assets/people_1.png" />
              </slide>
              <slide>
                <img src="@/assets/people_2.png" />
              </slide>
            </carousel>
          </div>
        </div>
        <div class="col-sm"></div>
      </div>
    </div>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
export default {
  name: "home",
  components: {
    Carousel,
    Slide,
  },
};
</script>

<style lang="css" scoped>
.card {
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  flex-direction: column;
  min-width: 0;
  background-color: #fff;
  background-clip: border-box;
  border: 0.0625rem solid rgba(0, 0, 0, 0.05);
  border-radius: 0.25rem;
}
.slider {
  width: 73%;
  border-radius: 1rem;
  margin: 20% 15%;
  box-shadow: 0 15px 35px rgba(50, 50, 93, 0.1), 0 5px 15px rgba(0, 0, 0, 0.07) !important;
}
img {
  width: 60rem;
  height: 17rem;
}
.VueCarousel-slide {
  text-align: center;
}
</style>
