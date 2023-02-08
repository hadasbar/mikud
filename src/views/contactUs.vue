<template>
  <div class="contact-container main-layout">
    <div class="contact-titles">
      <h1>צרו קשר</h1>
      <h4 class="sub-title">השאירו פרטים ונחזור אליכם בהקדם</h4>
    </div>

    <div class="contact-form-container">
      <div class="contact-info">
        <h3 class="no-margin-top">?איפה אנחנו נמצאים</h3>

        <div class="mapouter">
          <div class="gmap_canvas">
            <iframe
              class="gmap_iframe"
              width="100%"
              frameborder="0"
              scrolling="no"
              marginheight="0"
              marginwidth="0"
              src="https://maps.google.com/maps?width=600&amp;height=auto&amp;hl=en&amp;q=עוזיאל 41 גבעת שמואל&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"
            ></iframe>
            <!-- <a href="https://pdflist.com/" alt="pdf download">Pdf download</a> -->
          </div>
        </div>

        <h3>דרכי התקשרות</h3>
        <div class="contacts">
          <div>עוזיאל 41, גבעת שמואל &nbsp;<i class="fa-sharp fa-solid fa-location-dot"></i></div>
          <div>mikud.studycenter@gmail.com &nbsp;<i class="fa-solid fa-envelope"></i></div>
          <div>054-3210400 &nbsp;<i class="fa-solid fa-phone"></i></div>
        </div>
      </div>

      <form class="contact-form">
        <input type="text" placeholder="שם מלא " />
        <input type="text" placeholder="מספר טלפון" />
        <textarea id="" cols="30" rows="10" placeholder="ספרו לנו עוד"></textarea>

        <button class="submit-form-btn">שלח</button>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  components: {},
  data: () => {
    return {}
  },
  methods: {},
  computed: {},
}
</script>

<style>
.mapouter {
  position: relative;
  text-align: right;
  width: 100%;
  height: 100%;
}
.gmap_canvas {
  overflow: hidden;
  background: none !important;
  width: 100%;
  height: 100%;
}
.gmap_iframe {
  height: 100% !important;
}
</style>
