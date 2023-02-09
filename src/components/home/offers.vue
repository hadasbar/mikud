<template>
  <div class="offer-layout">
    <div class="main-layout offer-container">
      <h1>מה אנחנו מציעים?</h1>
      <!-- <h4>אנו במיקוד מאמינים בהשגת פועלים מתחושת שליחות תוך יצירת בלה בלה ממש רציני</h4> -->
      <div class="offer-list">
        <div v-for="offer in offers" key="offers.indexOf(offer)" class="offer">
          <img class="offer-gif" :src="offer.icon" alt="" />
          <h4>{{ offer.title }}</h4>
          <h6 class="offer-description">{{ offer.description }}</h6>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      offers: [
        {
          icon: '../../src/styles/imgs/Reading-Book.gif',

          title: 'ביהס לעברית',
          description: ' ביה"ס לעברית מציע מגוון רחב של שיעורים המלמדים בלה בלה',
        },
        {
          icon: '../../src/styles/imgs/Creative-Thinking.gif',
          title: 'סטודנטים',
          description: 'אנחנו כאן להציע מרתונים לפני המבחנים, ושיעורים פרטיים במהלך הסמסטר',
        },
        {
          icon: '../../src/styles/imgs/Web-Browsing.gif',

          title: 'ביה"ס לאנגלית',
          description: 'ביה"ס לאנגלית מציע מגוון  שיעורי אנגלית לשיפור הדיבור  והכתיבה',
        },
        {
          icon: '../../src/styles/imgs/Form-Filling.gif',

          title: 'שיעורים פרטיים',
          description: 'צוות מורים מקצועיים המכינים מערכי שיעור מותאמים לרמת התלמיד ותכנית התקדמות',
        },
        {
          icon: '../../src/styles/imgs/Online-Study.gif',
          title: 'מרכז בגבעת שמואל',
          description: 'המון דברים ממש כיפיים  ולימודיים מתרחשים פה',
        },
        {
          icon: '../../src/styles/imgs/Telescope.gif',

          title: 'תוכנית גפן',
          description: 'אני כאן כל הזמן',
        },
      ],
    }
  },
  created() {},
  methods: {},
  computed: {},
  unmounted() {},
}
</script>
<style></style>
