<template>
  <div class="main-layout flex review-container">
    <button class="left-btn review-btn" @click="moveReview(-1)"><i class="fa-solid fa-chevron-left"></i></button>

    <div class="flex img-txt-cont">
      <!-- <img class="review-img" :src="reviewImg" alt="no" /> -->

      <div class="review-txt">
        <!-- <h1 class="quote">"</h1> -->
        <svg class="quote-svg" xmlns="http://www.w3.org/2000/svg" data-name="Layer 1" viewBox="0 0 128 128">
          <path
            d="M98.788 10.466a27.26 27.26 0 0 0-21.712 5.357 27.695 27.695 0 0 0 .12 44.405 27.276 27.276 0 0 0 25.509 4.324 1.33 1.33 0 0 1 1.25.186 1.364 1.364 0 0 1 .542 1.177c-1.249 27.64-26.037 38.446-30.994 40.332a3.658 3.658 0 0 0-2.323 3.937s.632 4.641.633 4.647a3.725 3.725 0 0 0 4.987 2.916c56.567-22.964 52.526-64.727 49.94-76.98-2.64-12.504-12.513-27.32-27.952-30.301zm4.49 18.086a2.002 2.002 0 0 1-2.815-.298c-4.287-5.303-11.658-2.548-11.733-2.518a2 2 0 1 1-1.437-3.734c.413-.159 10.184-3.805 16.283 3.737a2 2 0 0 1-.299 2.813zm-70.49-18.086a27.26 27.26 0 0 0-21.712 5.357 27.695 27.695 0 0 0 .12 44.405 27.276 27.276 0 0 0 25.509 4.324 1.33 1.33 0 0 1 1.25.186 1.364 1.364 0 0 1 .542 1.177c-1.249 27.64-26.037 38.446-30.994 40.332a3.658 3.658 0 0 0-2.323 3.937s.632 4.641.633 4.647a3.725 3.725 0 0 0 4.987 2.916c56.567-22.964 52.526-64.727 49.94-76.98-2.64-12.504-12.513-27.32-27.952-30.301zm4.49 18.086a2.054 2.054 0 0 1-2.815-.299c-4.287-5.302-11.658-2.547-11.733-2.518a2 2 0 1 1-1.437-3.733c.413-.159 10.184-3.805 16.283 3.737a2 2 0 0 1-.299 2.813z"
            fill="#ffa216"
            class="color000000 svgShape"
          ></path>
        </svg>
        <h6 class="review-description">{{ reviews[i].reviewDscription }}</h6>
        <h1 class="review-name">{{ reviews[i].reviewName }}</h1>
        <h1 class="review-info">{{ reviews[i].reviewInfo }}</h1>
      </div>
    </div>

    <button class="right-btn review-btn" @click="moveReview(+1)"><i class="fa-solid fa-chevron-right"></i></button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      i: 0,

      reviews: [
        {
          reviewDscription:
            'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illum, veritatis voluptatibus distinctio impedit eligendi.',
          reviewName: 'חגית כהן,',
          reviewInfo: 'אמא של תלמיד כיתה ד עולה חדש ממקסיקו',
        },
        {
          reviewDscription:
            'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illum, veritatis voluptatibus distinctio impedit eligendi qui similique tenetur.',
          reviewName: 'עדינה וינשטוק,',

          reviewInfo: 'שני תלמידת גיתה י"א, 4 יחידות מתמטיקה',
        },

        {
          reviewDscription:
            'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Illum, veritatis voluptatibus distinctio impedit eligendi qui similique tenetur neque aliquid accusantium velit suscipit accusamus inventore .',
          reviewName: 'דניאלה איליה,',

          reviewInfo: 'עדי, סטודנטית להנדסת חשמל בבר אילן אחרי מבחן בחדו"א 1',
        },

        ,
      ],
    }
  },
  created() {},
  methods: {
    moveReview(dif) {
      var currNum = this.i + dif
      console.log('currNum', currNum)
      if (currNum === 3) {
        this.i = 0
      } else if (currNum === -1) {
        this.i = 2
      } else {
        this.i = currNum
      }
    },
  },
  computed: {
    reviewImg() {
      return `../../src/styles/imgs/review${this.i}.jpeg`
    },
  },

  unmounted() {},
}
</script>
<style></style>
