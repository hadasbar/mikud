<template>
  <header class="header">
    <nav class="main-layout">
      <RouterLink class="header-item" to="/contactUs"> עברית </RouterLink>
      <RouterLink class="header-item" to="/contactUs">
        <div>אנגלית</div>
      </RouterLink>
      <RouterLink class="header-item" to="/contactUs">
        <div>סטודנטים</div>
      </RouterLink>
      <RouterLink class="header-item" to="/contactUs">
        <div>צור קשר</div>
      </RouterLink>
      <RouterLink class="header-item" to="/">
        <div>שאלות נפוצות</div>
      </RouterLink>
      <RouterLink class="header-item" to="/">
        <div>אודות</div>
      </RouterLink>
      <RouterLink class="header-item" to="/">
        <div>השיטה</div>
      </RouterLink>
      <RouterLink class="header-item" to="/">
        <div>קורסים</div>
      </RouterLink>
      <RouterLink class="header-item" to="/">
        <div>מרכזים</div>
      </RouterLink>
      <RouterLink class="header-item" to="/">
        <div>התחברות</div>
      </RouterLink>
    </nav>
  </header>
</template>
<script>
export default {
  components: {},
  data: () => {
    return {
      contact: '/contactUs',
    }
  },
  methods: {},
  computed: {},
}
</script>
