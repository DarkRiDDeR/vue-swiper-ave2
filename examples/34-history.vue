<template>
  <md-card>
    <md-card-actions>
      <div class="md-subhead">
        <span>History API</span>
        <span>（</span>
        <span>历史记录</span>
        <span>）</span>
      </div>
      <md-button
        class="md-icon-button"
        target="_blank"
        href="https://github.com/DarkRiDDeR/vue-swiper-ave2/blob/master/examples/34-history.vue"
      >
        <md-icon>code</md-icon>
      </md-button>
    </md-card-actions>
    <md-card-media>
      <!-- swiper -->
      <swiper :options="swiperOption">
        <swiper-slide>Slide 1</swiper-slide>
        <swiper-slide>Slide 2</swiper-slide>
        <swiper-slide>Slide 3</swiper-slide>
        <swiper-slide>Slide 4</swiper-slide>
        <swiper-slide>Slide 5</swiper-slide>
        <swiper-slide>Slide 6</swiper-slide>
        <swiper-slide>Slide 7</swiper-slide>
        <swiper-slide>Slide 8</swiper-slide>
        <swiper-slide>Slide 9</swiper-slide>
        <swiper-slide>Slide 10</swiper-slide>
        <div
          class="swiper-pagination"
          slot="pagination"
        />
        <div
          class="swiper-button-prev"
          slot="button-prev"
        />
        <div
          class="swiper-button-next"
          slot="button-next"
        />
      </swiper>
    </md-card-media>
  </md-card>
</template>

<script>
  export default {
    data() {
      return {
        swiperOption: {
          spaceBetween: 50,
          slidesPerView: 1,
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev'
          },
          pagination: {
            el: '.swiper-pagination'
          },
          history: {
            key: 'slide'
          }
        }
      }
    }
  }
</script>
