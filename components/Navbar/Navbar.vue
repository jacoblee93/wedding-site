<template>
  <div class="navbar">
    <NavbarItem v-for="navbarItem in navbarItems" :key="navbarItem.title" :title="navbarItem.title" />
  </div>
</template>

<style>
  .navbar {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 64px;
    width: 100%;
    background: var(--parchment-light);
    position: fixed;
    top: 0;
    z-index: 1;
  }
</style>

<script>
export default {
  data() {
    return {
      navbarItems: [{
        title: 'Our Story'
      }, {
        title: 'Gallery'
      }, {
        title: 'Weekend Details'
      }, {
        title: 'Registry'
      }, {
        title: 'TODO in Napaaaah'
      }, {
        title: 'RSVP'
      }]
    }
  }
}
</script>