<template>
  <div id="app">
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <figure class="image center">
            <img src="./assets/8.gif" style="max-width: 96px;">
          </figure>
          <h1 class="title center">News</h1>
        </div>
      </div>
    </section>
    <router-view/>
  </div>
</template>

<style>

.center {
  display: flex!important;
  justify-content: center!important;
  align-items: center!important;
}

</style>
