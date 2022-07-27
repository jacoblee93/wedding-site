<template>
  <div class="navbar-item">
    <a :href="'/#'+ linkHash">{{title}}</a>
  </div>
</template>

<style>
  .navbar-item {
    margin: 4px 8px;
  }
</style>

<script>
export default {
  props: ['title'],
  data() {
    return {
    };
  },
  computed: {
    linkHash: function () {
      return this.title.toLowerCase().replace(/ /gi, '');
    }
  }
}
</script>