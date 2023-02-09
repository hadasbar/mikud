<template>
  <div class="about-us">
    <img class="orange-wave" src="../../styles/imgs/orangeWave.png" alt="" />
    <div class="main-layout">
      <h1 class="about-title">? מי אנחנו</h1>
      <h6 class="about-sub-title">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere libero veritatis quas ex ut commodi explicabo at ipsam dicta.
      </h6>

      <div class="flex about-info-cont">
        <div class="about-info">
          &quot;מיקוד&quot; מרכז למידה הוא מרכז המציע שיעורים פרטיים וקבוצות למידה לתלמידים כיתות א עד יב, כמו כן גם לסטודנטים. במרכז זה יש
          מרכז ראשי בגבעת שמואל, שמוביל חוויות למידה מועילות ומתאימות לצרכי כל תלמיד. כמו כן, מיקוד מרכז למידה מקיים שיתופי פעולה עם בתי ספר
          וחוויות למידה מאופיינות להפעלה ולהשתתפות בלמידה המועילה ביותר. מורי המרכז מקצועיים ונדיבים, ומאמינים באינטראקציה מול התלמידים כדי
          להביא אותם לדרך לימוד המוצלחת.
        </div>
        <svgg class="about-svg" />
      </div>
    </div>
  </div>
</template>
<script>
import svgg from './svgs/svg-aboutus.vue'

export default {
  components: { svgg },
  data: () => {
    return {}
  },
  methods: {},
  computed: {},
}
</script>
