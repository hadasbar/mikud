<template>
  <section class="f">
    <RouterLink class="logo" to="/">
      <img class="logo" src="../src/styles/imgs/logo.png" alt="" />
    </RouterLink>
    <appHeader> </appHeader>

    <RouterView />
    <appFooter></appFooter>
    <appContact :class="[isHeaderWhite ? 'display-contact' : 'dont-display-contact']"></appContact>
    <!-- 
        :class="[checkHomeRoute ? 'header-transparent' : 'header-white', checkHomeRoute && isHeaderWhite ? 'bg-white' : '']" -->
  </section>
</template>

<script>
import { RouterLink, RouterView } from 'vue-router'
import appHeader from './components/header.vue'
import appFooter from './components/footer.vue'
import appContact from './components/app-contact.vue'

export default {
  components: {
    appHeader,
    appFooter,
    appContact,
  },
  data: () => {
    return {
      isHeaderWhite: false,
    }
  },
  methods: {
    handleScroll(ev) {
      this.isHeaderWhite = true
      if (window.scrollY === 0) this.isHeaderWhite = false
    },
  },

  computed: {
    checkHomeRoute() {
      const path = this.$route.path.split('/')
      console.log('path', path)
      return path[path.length - 1].toLowerCase() === ''
    },
  },
  created() {
    window.addEventListener('scroll', this.handleScroll)
  },
  destroyed() {
    window.removeEventListener('scroll', this.handleScroll)
  },
}
</script>
<style>
.f {
  position: relative;
}
.logo {
  position: fixed;
  top: 0;
  right: 0;
}

.display-contact {
  /* bottom: 100vh; */
  display: block;
}

.dont-display-contact {
  /* bottom: 0; */
  display: none;
}
/* .f {
  height: auto;
}
.header-transparent {
  background-color: rgba(246, 8, 8, 0);
  position: sticky;
  top: 0;
  z-index: 99;
  color: rgb(255, 255, 255);
}

.header-white {
  background-color: rgb(255, 255, 255);
  color: rgb(109, 105, 105);
}

.bg-white {
  background-color: rgb(255, 255, 255);
  position: sticky;
  top: 0;
  z-index: 99;
  color: pink;
} */
</style>
