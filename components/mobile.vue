<template>
  <div style="width: 200px">
    <client-only>
      <swiper :options="swiperOption">
        <swiper-slide>
          <img width="200" src="@/assets/img/1.png" />
        </swiper-slide>
        <swiper-slide>
          <img width="200" src="@/assets/img/2.png" />
        </swiper-slide>
        <swiper-slide>
          <img width="200" src="@/assets/img/3.png" />
        </swiper-slide>
        <swiper-slide>
          <img width="200" src="@/assets/img/4.png" />
        </swiper-slide>
        <swiper-slide>
          <img width="200" src="@/assets/img/5.png" />
        </swiper-slide>

        <div class="swiper-pagination" slot="pagination"></div>
      </swiper>
    </client-only>
  </div>
</template>

<script>
export default {
  data() {
    return {
      swiperOption: {
        autoplay: {
          delay: 2500,
          disableOnInteraction: false,
        },
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
      },
    };
  },
};
</script>
<style>
.swiper-pagination-bullet {
  background: #fff;
}
.swiper-pagination-bullet-active {
  background: #ffa31a;
}
</style>
