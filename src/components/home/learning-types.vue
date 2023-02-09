<template>
  <main class="learning-types main-layout">
    <div>
      <div class="learning-titles">
        <h1>מה תמצאו אצלנו?</h1>
        <h6 class="sub-title"></h6>
      </div>

      <div class="learning-items">
        <div class="learning-item">
          <img src="../../../src/styles/imgs/private-lesson.png" alt="" />

          <div class="learning-item-info">
            <h3>שיעורים פרטיים</h3>
            <div class="flex space-between">
              <h6>מספר תלמידים: 1</h6>
              <h6>ע"י: עדי</h6>
            </div>
            <p>
              {{ lorem }}
            </p>
          </div>
        </div>
        <div class="learning-item">
          <img src="../../../src/styles/imgs/wwww.png" alt="" />

          <div class="learning-item-info">
            <h3>מרתונים</h3>

            <div class="flex space-between">
              <h6>מספר תלמידים: עד 5</h6>
              <h6>ע"י: עדי</h6>
            </div>
            <p>
              {{ lorem }}
            </p>
          </div>
        </div>
        <div class="learning-item">
          <img src="../../../src/styles/imgs/zoom-call.png" alt="" />
          <div class="learning-item-info">
            <h3>למידה מרחוק</h3>

            <div class="flex space-between">
              <h6>מספר תלמידים: 1</h6>
              <h6>ע"י: עדי</h6>
            </div>
            <p>
              {{ lorem }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  components: {},
  data: () => {
    return {
      lorem:
        ' Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex consequatur, quam ut optio quisquam dolorem maiores perspic totam cupiditate asperiores provident praesentium nesciunt aperiam ipsam reiciendis aliquid adipisci sit beatae',
    }
  },
  methods: {},
  computed: {},
}
</script>
