<template>
  <div class="index-page">
    <Navbar />
    <section class="omg-its-us">
      <img src="~/static/images/dance.jpg">
      <div class="need-to-know">
        <h1 class="who">
          Lena Maria and Jacob
        </h1>
        <h3 class="where its-at">
          Napa, California
        </h3>
        <h3 class="when its-at">
          June 10th, 2023
        </h3>
      </div>
    </section>
    <section class="image" id="ourstory">
      <Timeline />
    </section>
  </div>
</template>

<style>
  .index-page {
    display: flex;
    flex-direction: column;
    background: var(--parchment-light);
  }
  section {
    display: flex;
    align-items: center;
    flex-direction: column;
  }
  .omg-its-us {
    width: 100%;
  }
  .omg-its-us img {
    object-fit: cover;
    height: 100vh;
    width: 100%;
  }
  .omg-its-us .need-to-know {
    position: absolute;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    margin-top: 64px;
    margin-right: 48px;
    width: 100%;
  }
  .its-at {
    margin: 0;
  }
  .image {
    height: 1000vh;
    width: 100%;
  }
  /* .image {
    background: url("~/static/images/kite.jpg")
  } */
</style>

<script>
export default {
  name: 'IndexPage'
}
</script>
