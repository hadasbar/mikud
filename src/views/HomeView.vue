<template>
  <div class="home-page">
    <open />

    <offers />

    <aboutUs />
    <ourWays />

    <learningTypes />

    <reviews />
  </div>
</template>
<script>
import open from '../components/home/open.vue'
import offers from '../components/home/offers.vue'
import aboutUs from '../components/home/about.vue'
import learningTypes from '../components/home/learning-types.vue'
import reviews from '../components/home/reviews.vue'
import ourWays from '../components/home/our-ways.vue'

export default {
  components: { open, offers, aboutUs, learningTypes, reviews, ourWays },
  data: () => {
    return {}
  },
  methods: {},
  computed: {},
}
</script>

<style></style>
