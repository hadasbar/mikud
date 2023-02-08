<template>
  <div class="main-layout flex review-container">

    <button class="left-btn review-btn" @click="moveReview(-1)"><i class="fa-solid fa-chevron-left"></i></button>
    <div class="flex img-txt-cont">
      <img class="review-img" :src="reviewImg" alt="no" />
      <div class="review-txt">
        <h6 class="review-txt-sub">{{ reviews[i].reviewDscription }}</h6>
        <h1 class="review-txt-title">{{ reviews[i].reviewInfo }}</h1>
        <!-- {{ reviews[i] }} -->
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
        { reviewDscription: '4 שעות עברית בשבוע | במרכז למידה ברעננה', reviewInfo: 'אמא של תלמיד כיתה ד עולה חדש ממקסיקו' },
        { reviewDscription: 'שיעור אחד בשבוע | בבית בתלמידה', reviewInfo: 'שני תלמידת גיתה י"א, 4 יחידות מתמטיקה' },

        { reviewDscription: 'שיעור 1 בשבוע לאורך הסמסטר |   זום', reviewInfo: 'עדי, סטודנטית להנדסת חשמל בבר אילן אחרי מבחן בחדו"א 1' },

        ,
      ],
    }
  },
  created() { },
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

  unmounted() { },
}
</script>
<style>

</style>
